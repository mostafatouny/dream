# `z-docker-opam`

<br>

This example runs a simple Web app inside a [Docker](https://www.docker.com/) container using [opam](https://opam.ocaml.org/) as the package manager. The Dockerfile has a build stage based on [opam base images](https://hub.docker.com/r/ocaml/opam) and a run stage based on [alpine](https://hub.docker.com/_/alpine)

Build the image `hello-dream` from `Dockerfile`
```
docker build . --tag hello-dream
```

create and run the container `hello-dream-container` with the image `hello-dream`
```
docker run --name hello-dream-container -p 8080:8080 hello-dream:latest
```

See also [**`z-docker-esy`**](../z-docker-esy) for using the `esy` package manager and `Docker compose`.

<br>

[Up to the example index](../#deploying)
