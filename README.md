# Yapper: Yet Another Pet Project En Route

Yapper is a collection of pet project ideas that are good for learning or short hacking sessions. If you want to build something but don't have time to come up with a project idea, this book has you covered.

Each project is designed to be self-contained and can be completed in a few hours to a few days, depending on your experience level.

Click here for the [**live book**](https://yapper.vincevarga.dev).

## Prerequisites

Make sure you have the following tools installed:

- **Rust**: Install from [rustup.rs](https://rustup.rs/)
- **mdBook**: Install with `cargo install mdbook`

## Building Locally

To build the book:

```bash
mdbook build
```

This generates the static site in the `book/` directory.

## Serving Locally

To serve the book locally with live reload:

```bash
mdbook serve
```

Then open your browser and navigate to `http://localhost:3000` to view the book. Changes to the source files will automatically trigger a rebuild and refresh.

You can also specify a different port:

```bash
mdbook serve --port 8080
```

## Deployment

This project is deployed to a Scaleway server using a release script. The deployment uses Caddy as the web server.

### Release Process

To deploy the book, run:

```bash
./release.sh
```

For additional debug output and health checks:

```bash
./release.sh --debug
```

### What the Release Script Does

1. **Builds the mdBook** using `mdbook build`
2. **Backs up the existing deployment** on the server
3. **Copies the Caddy configuration snippet** to `/etc/caddy/conf.d/yapper.vincevarga.dev.caddy`
4. **Deploys the `book/` directory** to `/var/www/yapper.vincevarga.dev/`
5. **Reloads Caddy** to apply any configuration changes
6. **Cleans up old backups** (keeps the latest 5)

## License

This project is licensed under the MIT License.

