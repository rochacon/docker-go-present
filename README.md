# Docker Go Present

Docker Go Present is a Docker base image that makes it easy to run and share your Go presentations build with [Present](https://code.google.com/p/go/source/browse/?repo=tools#hg%2Fcmd%2Fpresent).

## Usage

* Create a Dockerfile in your presentation directory with the following contents:

```
FROM rochacon/go-present
```

* Build your container

```
docker build -t my-cool-presentation .
```

## Run your presentation

Start your dockerized presentation.

```
docker run -d -p 3999:3999 my-cool-presentation
```

## Share your presentation

Now that your presentation is dockerized, upload it to the [Docker Hub](https://hub.docker.com/) and share it with the world!

```
docker push my-cool-presentation
```
