---
description: >-
  Learn about the main limitations of Node.js, especially in CPU-bound tasks,
  and how to overcome them using available strategies.
---

# Limitations and How to Handle Them

Node.js is **not great** for everything.

## The Problem:

* CPU-intensive operations (image processing, data crunching) can **block the event loop**.
* This means all requests freeze.

## Solutions:

* `worker_threads` module (built-in)
* `child_process` to spawn external work
* Use microservices for heavy tasks
* Offload to cloud functions
