## Docker Notes

- `docker build -t <tag> .`  
  Build image from current dir, name it with `<tag>`

- `docker run <image>`  
  To run + turn image to container and its for the fast resultes programmes

- `docker run -p 8080:8080 -d <image>`  
  To run + turn image to container and its just for the listning programmes

- `docker ps`  
  Shows all the containers who are running

- `docker ps -a`  
  Shows all the containers (-a = --all)

- `docker ps -a -f "status=exited"`  
  Shows all the containers who are not running (-f = --filter)

- `docker rename <old> <new>`  
  To Rename a Container

- `docker system prune`  
  Removes all stopped containers, unused images, volumes, networks

- `docker image prune`
  Removes all the <none> images

- `docker container prune`  
  Removes all the unrunning containers

- `docker exec -it <ID> sh`  
  To enter the terminal of the container (i = --interactive, t = --terminal)
