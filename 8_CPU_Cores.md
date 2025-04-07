# How Node.js Utilizes CPU Cores

Out of the box, Node.js runs on **one CPU core**. But modern CPUs have many.

## 🧠 Strategies to Scale:

- **Cluster module**: Run multiple Node.js processes
- **PM2**: Process manager for clustering, monitoring
- **Docker + Load Balancing**: Perfect for scalable production

## 💡 Smart Design:

Run one Node.js process per core.  
Use a load balancer to route requests.  
Boom — multi-core scalability achieved.
