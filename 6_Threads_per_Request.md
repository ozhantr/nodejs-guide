# Why Node.js Doesn’t Use Threads Per Request

Unlike Java or PHP, Node.js doesn't create a new thread for each HTTP request.

## 🔄 Traditional Server (e.g. Apache):

- Each request spawns a thread
- More threads = more RAM
- High context-switching cost

## 💡 Node.js Approach:

- One thread handles all requests
- Asynchronous delegation = less memory usage
- Scales to 10k+ concurrent users easily
