## Course Overview:
![1.png](./images/1.png)

---

## What is Docker:
![2.png](./images/2.png)

---
## What is a Container:
![3.png](./images/3.png)

---
## Docker *Image* vs *Container* :
![4.png](./images/4.png)

---

## *Docker* vs *Virtual Machine* :
![5.png](./images/5.png)

---

- OS has 2 layers:
    1. *OS Kernel Layer* : It communicates with hardware.
    1. *Application Layer* : All applications run on **kernel** layer.

![6.png](./images/6.png)

---

- Differences between docker and VM:
    1. *Size* : Docker image is much smaller.
    1. *Speed* : Docker containers start and run much fast.
    1. *Compatibility* : VM of any OS can run on any OS host.

![7.png](./images/7.png)

---

## Basic docker commands:

- `docker run image:version` -> this cmd downloads the the image.
- `docker run -d` -> run in *detached* mode, so we can use terminal again.
- `docker run -p6000:6379` -> bind *container* port to *host* post.
- `docker run --name redis-older redis:4.0` -> will create a new container, named as `redis-older`
- `docker images` -> to see all the images that we've locally.
- `docker ps` -> to see the running containers.
- `docker ps -a` -> to see all containers (both running and turned off).
- `docker start container_id`
- `docker stop container_id`
 
![8.png](./images/8.png)
### Docker commands

---

## **Container** port vs **Host** port:

- `docker run -p6000:6379 redis`
    - here `6000` is **host port**.
    - here `6379` is **container port**.
    - `redis` is the *image* name that will be pulled from docker hub.

![9.png](./images/9.png)

---

## Debugging a container:
57 mins 15 sec

- `docker logs container_name`
- `docker logs container_id`
- `docker exec -it container_id /bin/bash` (clearly bujhi nai)
- `docker exec -it container_name /bin/bash` (clearly bujhi nai)


