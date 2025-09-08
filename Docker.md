
## Docker Notes

# Why docker was envented 

**Docker was invented because at first there was a problem with hosting — if they wanted to host an app, they could do it on one server, but they couldn’t host two on the same server due to (security, conflicts, resource limits). That’s why they invented VMs, so they could run multiple OSs on a single server and host many apps based on hardware limits. Then they found a second problem: VMs use too many resources. That’s why they invented Docker to solve all those problems with something called containerization.**

```bash
docker build -t <tag> .
```  
**`docker build`** builds an image from the current directory and names it with `<tag>`.

```bash
docker run <image>
```  
**`docker run`** runs an image and creates a container, useful for quick tests.

```bash
docker run -p 8080:8080 -d <image>
```  
**`docker run -p`** maps ports and runs the container in detached mode (for listening services).

```bash
docker ps
```  
**`docker ps`** shows running containers.

```bash
docker ps -a
```  
**`docker ps -a`** shows all containers, including stopped ones.

```bash
docker ps -a -f "status=exited"
```  
**`docker ps -a -f`** filters and shows only exited (stopped) containers.

```bash
docker rename <old> <new>
```  
**`docker rename`** renames a container.

```bash
docker system prune
```  
**`docker system prune`** removes all unused containers, images, volumes, and networks.

```bash
docker image prune
```  
**`docker image prune`** removes dangling images (`<none>`).

```bash
docker container prune
```  
**`docker container prune`** removes all stopped containers.

```bash
docker exec -it <ID> sh
```  
**`docker exec -it`** lets you enter the container's terminal (`-i` interactive, `-t` terminal).

```bash
docker rmi $(docker images -q)
```  
**`docker rmi`** removes all Docker images by ID.

```bash
docker inspect <image>
```
**`docker inspect`** To see all the meta data for the image.

```bash
ENV VARIABLE_NAME = value
```
**`ENV VARIABLE_NAME = value`** To put envirment variables inside the Docker file.