# My Docker Notes (Beginner)

## 1. The Core Idea

The goal of Docker is to package an application and all its requirements into a standardized "box" that can run anywhere.

- **Image** 📜: The blueprint or recipe. It’s a saved, unchangeable package.
  - *Example:* The official `nginx` blueprint.
- **Container** 📦: A running instance created from an Image. It's the actual "box" that is running your application.
  - *Example:* The `my-web-server` container you created.

> **Analogy:** An **Image** is a recipe for a cake. A **Container** is the actual cake you baked. You can bake many cakes (containers) from one recipe (image).

## 2. Essential Commands

#### Verifying Your Setup
This is the first command to run. It downloads a test image and runs a container to confirm everything works.
```bash
docker run hello-world


####################################################################################

Running a Service (like a Web Server)

--- This is how you run a useful, long-running application.
------- Bash

docker run --publish 8080:80 --detach --name my-web-server nginx


Command Breakdown:

    --publish 8080:80: Connects your computer's port 8080 to the container's port 80.

    --detach: Runs the container in the background.

    --name my-web-server: Gives your container a custom, easy-to-remember name.

    nginx: The name of the image to use.
    
####################################################################################################

Managing Your Containers
----- These commands help you see and control your containers.
-------- Bash

# See all containers that are CURRENTLY RUNNING
docker ps

# See ALL containers on your system (including stopped ones)
docker ps -a

# Stop a running container by its name
docker stop my-web-server

# Permanently remove a STOPPED container by its name
docker rm my-web-server
