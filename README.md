# docker-alpine-catboost
An [Alpine Linux](https://hub.docker.com/_/alpine/) based docker image capable of running [Yandex CatBoost](https://tech.yandex.com/catboost/) with the open source [Anaconda distribution](https://www.anaconda.com/distribution/). 

## Template
Build your own image by creating a `Dockerfile`. A sample template that sets up a simple jupyter server has been provided below.
```
FROM valiantone/alpine-conda:latest

conda install jupyter[notebook]
EXPOSE 8888

CMD["jupyter", "notebook"]
```
