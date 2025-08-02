
## Docker Notes

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