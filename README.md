# some_docs

```
git clone git@github.com:thiskevinwang/some_docs.git
cd some_docs
```

## Prerequisites

`docker` CLI

## Get Started

### Run an instance of `nomad` website

This docker image contains no `content` and the `/docs` route will not work. The base route `/` will work though.

```
docker run --rm -p 3000:3000 --name=my_container thekevinwang/nextjs-docker
```

### Feed it some `content`

In a separate terminal window

```
docker cp content/. my_container:/app/content
```

Go to `localhost:3000`, refresh, and view docs
