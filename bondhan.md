clone this repo and run below:

```bash
$ YARN_OPTS='--network-timeout 10000000' docker compose -f docker/docker-compose-redis-os-test.yaml up --build --force-recreate -d
```

clone the worker repo:

```bash
git clone https://github.com/bondhan/client-conductor-worker
```
and then:

```bash
$ docker build -t worker:latest -f Dockerfile .
$ cd server && docker build -t server:latest -f Dockerfile .
```

evidences in folder _evidences_