# simplehttpserver

A simple http server written in C++ based on Boost.Beast.

## Build docker

```bash
docker build . -t mostsignificant/simplehttpserver
```

## Run docker container

```bash
docker run \
  --mount type=bind,source="$(pwd)",target=/var/www \
  -p 8080:8080 \
  -d \
  mostsignificant/simplehttpserver:latest
```

## Reference

[Christian Göhring, A Practical Guide To Containerize Your C++ Application With Docker](https://medium.com/codex/a-practical-guide-to-containerize-your-c-application-with-docker-50abb197f6d4)
