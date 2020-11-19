Make sure to replace $CONTAINER_ID with the container ID on your machine `docker ps`

- Run the ubuntu image with the process:

`docker run -d -ti ubuntu sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'`

- Get a shell inside the running container and install curl

`docker ps`

Run `docker logs $CONTAINER_ID` to see the logs, you should see the process awaiting input.

`docker exec -ti $CONTAINER_ID bash`

Run `apt-get update` followed by `apt-get install curl -y` to install curl

Exit `exit`

- Attach back to the running container and give input

`docker attach $CONTAINER_ID`

`ahmedgaber.org`

You see the response Moved Permanently