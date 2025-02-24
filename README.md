# dotnetcore_container

Wrapping .Net Core app in 🐳 container / Docker

## for development environment

```sh
$ docker build -f Dockerfile.dev . -t 103cuong/dotnetcore_container
$ docker run -it -v ${PWD}:/app -p 5001:5001 103cuong/dotnetcore_container
```

## for production environment

```sh
$ docker build . -t 103cuong/dotnetcore_container-prod
$ docker run -it -p 5001:443 -p 5000:80 103cuong/dotnetcore_container-prod
```
