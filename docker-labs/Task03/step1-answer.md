- Start the container in detached mode

`docker run -d devopsdockeruh/exec_bash_exercise`

- Get a shell inside the container and inspect logs

`docker ps` get container id

`docker exec -ti $CONTAINER_ID bash`

`tail -f ./logs.txt`