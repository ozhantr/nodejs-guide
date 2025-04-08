---
description: >-
  Understand the fundamental difference between processes and threads — key to
  grasping how Node.js handles concurrency.
---

# Process vs Thread: A Clear Distinction

Understanding how Node.js handles concurrency requires clarity on **processes** and **threads**.

## Definitions:

| Term        | Meaning                                                                                     |
| ----------- | ------------------------------------------------------------------------------------------- |
| **Process** | A running program. Isolated in memory, with its own resources.                              |
| **Thread**  | A unit of execution within a process. Shares memory with other threads in the same process. |

## Example:

* **Process**: Google Chrome = 1 process
* **Thread**: Inside Chrome, one thread handles UI, another loads pages, another handles audio, etc.
