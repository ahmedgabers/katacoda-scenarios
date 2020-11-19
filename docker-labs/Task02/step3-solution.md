1- Start a stopped container

  - List stopped containers
    `docker ps -a`

  - Run a stopped container
    `docker start 4ef717e9d2b3`


  - Replace 4ef717e9d2b3 with the container ID that has STATUS Exited

  - List running containers
    `docker ps`

Take a screen shot of the output and store in Day01/ directory


2- Run a container from ahmedgabercod/clock image in detached mode and attach to it

  - `docker run -d ahmedgabercod/clock`

  - `docker ps`

  - `docker attach 83eddd360892`

  - Replace 83eddd360892 with the container ID on your screen

  - You should see the out of the clock image
