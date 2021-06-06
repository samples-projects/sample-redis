# sample-redis

sample redis

## Up

```bash
$ docker-compose up -d
Creating network "sample-redis_default" with the default driver
Creating sample-redis_redis_1 ... done
```

## Usage

Enter to redis container

```bash
docker-compose exec redis /bin/bash
```

Execute redis-cli

```bash
$ redis-cli
127.0.0.1:6379> ping
PONG
127.0.0.1:6379> set test "HELLO, World!!"
OK
127.0.0.1:6379> get test
"HELLO, World!!"
127.0.0.1:6379> exit
```

## Down

```bash
$ docker-compose down
Stopping sample-redis_redis_1 ... done
Removing sample-redis_cli_1   ... done
Removing sample-redis_redis_1 ... done
Removing network sample-redis_default
```
