# RU202 - Redis Streams

<https://university.redislabs.com/courses/course-v1:redislabs+RU202+2019_03/course/>

Requirements:

* [Redis 5.x](https://docs.docker.com/samples/library/redis/)
* Python 3.6.5 (see [pyenv](https://github.com/pyenv/pyenv))

Setup:

* Make sure the following env variable are set: `REDIS_HOST`, `REDIS_PORT` and `PYTHONPATH`
* validate in the Terminal:

```
$ docker run --name redis-server \
  -p 127.0.0.1:6389:6379/tcp \
  -d redis:5-alpine redis-server \
  --appendonly yes
$ REDIS_PORT=6389 python helloworld.py
None
```
