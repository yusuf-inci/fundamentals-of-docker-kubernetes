# Commands

- Verify that docker CLI is installed.
`docker --version`
- Use the docker CLI to list your images.
`docker images`
- Pull your first image from Docker Hub.
`docker pull hello-world`
- Run the hello-world image as a container.
`docker run hello-world`
- List the containers to see that your container ran and exited successfully.
`docker ps -a`
- Remove specific container.
`docker container rm <container_id>`
- Build the image using Dockerfile
`docker build . -t myimage:v1`
- Run the image as a container.
`docker run -dp 8080:8080 myimage:v1`
- Run the curl command to ping the application as given below.
`curl localhost:8080`
- Stop the container we use docker stop followed by the container id. The following command uses docker ps -q to pass in the list of all running containers:
`docker stop $(docker ps -q)`
- Check if the container has stopped
`docker ps`
- Create a new tag for an existing image
`docker tag my-app:v1 second-app:v1`
- Build the Docker image and push it to Docker Hub
 $ docker build -t <docker-username>/<image-name:tag> .
 $ docker push <docker-username>/<image-name:tag>
 // $ docker build -t 90041/myimage:v1 . && docker push 90041/myimage:v1


| Command              | Description                                                        |
|----------------------|--------------------------------------------------------------------|
| docker build         | Builds an image from a Dockerfile.                                 |
| docker CLI           | Start the Docker command line interface.                           |
| docker container rm  | Removes a container.                                               |
| docker images        | Lists the images.                                                  |
| docker ps            | Lists the containers.                                              |
| docker pull          | Pulls the latest image or repository from a registry.              |
| docker push          | Pushes an image or a repository to a registry.                      |
| docker run           | Runs the <image name> in a new container.                           |
| docker run           | Runs a command in a new container.                                  |
| docker stop          | Stops one or more running containers.                               |
| docker tag           | Creates a tag for a target image that refers to a source image.     |
