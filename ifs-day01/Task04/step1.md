- Create a Dockerfile for a new image that starts from `ubuntu:16.04`

- Make a script file on you local machine with such content as:

  `echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;`

- Transfer this file to an image and run it inside the container using CMD

- Build the image with tag “curler”

- Run the command `docker run [options] curler` remember the flags (options) from Task03?

- Input ahmedgaber.org into it, output should match the previous task

Store the Dockerfile as 'Dockerfile.task04' in Day01/ directory