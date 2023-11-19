# docker_flask_homework

### Assignment:
- Course: HHA 504
- Homework assignment #7: Gain hands-on experience in Dockerizing Flask applications, first individually and then using Docker Compose for managing multiple applications.

### Part 1: Dockerizing a Single Flask Application
- Create a folder and name it `Part1`.
- Create a flask application within it.
- In addition, create a Docker file and name it `Dockerfile`. Copy [this code](https://github.com/Beczheng/docker_flask_homework/blob/main/Part1/Dockerfile).
- Lastly, create a text file and name it `requirements.txt`. Put `flask` in the file.
- In your Cloud Shell terminal, type `docker build -t <name of image> .`. This will build an image.
- Type `docker images`. This will show a list of your images.
- Type `docker run -d -p <port1>:<port2> <name of image>`. This will run the image in a container. 
- To preview your image, make sure to change your port to port 1 in Cloud Shell.
- Type `docker ps`. This will show a list of your containers.
- Type `docker stop <container ID>`. This will stop your container.
- Type `docker rm <container ID>`. This will remove your container.
- Type `docker system prune -a -f`. This will clean and remove everything.

### Part 2: Dockerizing Multiple Flask Applications (Using Compose)
- Create a folder a name it `Part2`.
- Create a Docker Compose file and name it `docker-compose.yaml` within it. Copy [this code](https://github.com/Beczheng/docker_flask_homework/blob/main/Part2/docker-compose.yaml).
- In addition, create two folders: `flask1` and `flask2`. Then, create a flask application for each folder.
- Include a Docker file in each folder. Name both files `Dockerfile`. Copy [this code](https://github.com/Beczheng/docker_flask_homework/blob/main/Part2/flask1/Dockerfile) for both.
- Include a `requirements.txt` file for each folder. Put `flask` in the files.
- In your Cloud Shell terminal, type `docker-compose build`. This will build your images.
- Type `docker-compose up`. This will run your images in containers.
- To preview your images, make sure to change your ports according to the Docker Compose file.
- Type `docker-compose ps`. This will show a list of your containers.
- Type `docker-compose down`. This will stop your containers.
- Type `docker system prune -a -f`. This will clean and remove everything.


