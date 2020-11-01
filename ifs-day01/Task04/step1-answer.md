```yaml
FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl

COPY script.sh /
RUN chmod +x /script.sh

CMD ["/script.sh"]
```

Run `docker build -t curler .` to build the image

Run `docker run -ti curler` to input the url

