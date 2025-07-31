## Docker Notes

- `docker build -t <tag> .`  
  Build image from current dir, name it with `<tag>`

- `docker run <image>`  
  Run container from image; runs and exits

- `docker run -p 8080:8080 <image>`  
  Maps port 8080 on host to 8080 in container
