# Instructions:

- Add Nginx in front of the fullstack

- Nginx will function as a reverse proxy for us

- The requests arriving at anything other than /api will be redirected to frontend container and /api will get redirected to backend container

- At the end you should see that the frontend is accessible simply by going to http://localhost and the button works

- Other buttons may have stopped working, do not worry about them


The following file should be set to /etc/nginx/nginx.conf inside the nginx container. You can use a file volume where the contents of the file are the following:

```yaml
  events { worker_connections 1024; }

  http {
    server {
      listen 80;

      location / {
        proxy_pass _frontend-connection-url_;
      }

      location /api/ {
        proxy_pass _backend-connection-url_;
      }
    }
  }
```

Note that again inside the docker-compose network the connecting urls are usually form “http://hostname:port” where hostname and port are both known only inside the network.

`Save the docker-compose.yml in Day01/ directory`