# Web Development & Modern Architecture Concepts

## HTTP & HTTP/2
- **HTTP/1.1**: One request per connection, slower with many requests.  
- **HTTP/2**: Multiplexing, header compression, server push; faster and more efficient.  
- Go `http.ListenAndServe` → HTTP/1.1, `ListenAndServeTLS` → HTTP/2 automatically.

## gRPC
- High-performance RPC framework by Google using HTTP/2 and Protocol Buffers.  
- Used for microservices, server-to-server communication, real-time APIs.  
- Works with any language; client-server communication is strongly typed.  

## AWS (Amazon Web Services)
- Cloud platform offering servers, databases, storage, networking, and more.  
- Helps deploy apps, host APIs, scale microservices, run databases.  

## Docker
- Packages apps with dependencies into **containers**.  
- Ensures consistency across environments.  

## Kubernetes
- Orchestrates containers: deployment, scaling, networking, self-healing.  
- Master/Worker architecture with **Pods** (container units) and **Services** (networking).  
- Supports horizontal (replicas) and vertical (more resources) scaling.  
- Can run locally (Minikube, Kind) or on cloud (EKS, GKE, AKS).  

## Microservices Professional Setup
- Containerize each service (Docker).  
- Use Kubernetes to manage deployment, scaling, and networking.  
- Internal communication: **gRPC** (fast) or **Kafka** (event-driven).  
- External clients: **REST/HTTP API**.  
- Add CI/CD, monitoring, and logging.  

## Kafka
- Distributed messaging system, handles high throughput and persistent events.  
- Producers send messages, consumers receive asynchronously.  
- Ideal for event-driven systems, real-time analytics, and microservices messaging.  

## Event-driven Architecture
- Apps react to events (e.g., “new order”).  
- Decouples services, good for async tasks.  

## Serverless (AWS Lambda)
- Run code on-demand without managing servers.  
- Useful for APIs, scheduled jobs, lightweight tasks.  

## WebSockets / gRPC Streams
- Real-time communication between client and server.  
- Use for chat, live updates, or real-time apps.  

## Prometheus + Grafana
- Monitor apps and visualize metrics (CPU, memory, requests).  
- Helps detect and fix issues.  

## Advanced CI/CD Pipelines
- Automate building, testing, and deploying apps.  
- Speeds up delivery, ensures reliability.  
