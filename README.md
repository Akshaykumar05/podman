# podman
This repo contains container (podman) learnings and hands-on.'

### To install Podman
```
yum install podman -y
```
```
alias docker=podman
```
```
podman -v
````
### Checking Podman Registries
```
podman info
```
  ```
  registries:
  search:
  - registry.access.redhat.com
  - registry.redhat.io
  - docker.io
  ```

### To serach for a image in registry
```
podman search nginx
```
### Checking already downloaded images
```
podman images
```
```
podman pull nginx
```
![image](https://github.com/user-attachments/assets/9f63cbec-b876-4c68-97b2-60648d5203d3)

### To download an image
```
podman pull docker.io/library/nginx
```
### To see the running container
```
podman ps
```


### Port Binding of container
```
podman run -dt -p 8080:80/tcp docker.io/library/nginx
```




