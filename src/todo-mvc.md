# TodoMVC

## What is it?

A todo list app. You add tasks, mark them as done, and delete them when you're finished. Simple.

TodoMVC is a classic in the web development world. The [TodoMVC project](https://todomvc.com/) has been around for over a decade, offering the same todo app implemented in dozens of JavaScript frameworks. It's used to compare frameworks, appears in browser benchmarks, and has become the "hello world" of frontend development.

If you're learning a new framework or language, this is often the first real project people recommend. And for good reason: it's small enough to finish in a day, but complex enough to touch most of the basics.

## Why build this?

- You'll learn how to manage state (a list of items that changes over time)
- You'll practice handling user input (adding, editing, deleting)
- You'll work with the DOM or your framework's way of rendering UI
- You'll think about data persistence (where do the todos go when you refresh?)

## Core features

Here's what a basic TodoMVC app should do:

1. **Add a todo** by typing in an input field and pressing Enter
2. **Mark a todo as complete** by clicking a checkbox
3. **Delete a todo** by clicking a remove button
4. **Edit a todo** by double-clicking on it
5. **Filter todos** by status: All, Active, Completed
6. **Clear all completed todos** with a single button
7. **Show the count** of remaining items

## Things to think about

- Where do you store the todos? In memory? LocalStorage? A database?
- What happens when you refresh the page?
- How do you handle empty states (no todos yet, no completed todos)?
- Can you add keyboard shortcuts?

## Take it further

Once you have the basics working, here are some ways to extend the project:

| Difficulty | Extension |
|------------|-----------|
| Easy | Persist todos to localStorage |
| Easy | Add due dates to todos |
| Medium | Sync across browser tabs |
| Medium | Add drag-and-drop reordering |
| Medium | Connect to a REST API backend |
| Hard | Real-time sync with multiple users |
| Hard | Implement offline-first with conflict resolution |
| Hard | Add CRDT-based collaborative editing |

## Reference

The official TodoMVC project has implementations in React, Vue, Angular, Svelte, and many more. Check out [todomvc.com](https://todomvc.com/) if you want to see how others have solved this problem, or use their app spec as a reference.
