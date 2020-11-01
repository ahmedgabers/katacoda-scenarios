Start a ubuntu image with the process sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'

You will notice that a few things required for proper execution are missing. Be sure to remind yourself which flags to use so that the read actually waits for input.

Use `docker .. --help` for help

Note also that `curl` is NOT installed in the container yet. You will have to install it from inside of the container.

