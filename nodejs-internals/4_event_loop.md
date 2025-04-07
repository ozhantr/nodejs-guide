---
description: >-
  A deep dive into the Node.js event loop — the engine that drives non-blocking,
  asynchronous operations.
---

# How the Event Loop Works

Node.js uses a **single-threaded event loop** to handle all tasks. Here's how it works:

1. Your code runs inside **one process**.
2. That process uses **one main thread**: the **event loop**.
3. Heavy I/O tasks (like reading files, hitting APIs) are passed to the background (`libuv`).
4. The event loop keeps checking: “Is anything done yet?”
5. When tasks finish, their callback is picked up and run.

## Visual Metaphor:

> Imagine a chef (event loop) managing 100 orders. Instead of cooking each dish himself, he delegates tasks to sous-chefs (libuv). He just checks when dishes are ready and sends them out.
