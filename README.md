## heroku-redisgreen

Heroku client plugin for [RedisGreen](https://addons.heroku.com/redisgreen).

### Installation

You'll need to install `redis-cli` locally first. This command comes with Redis
and can be downloaded from [redis.io](http://redis.io/download).

With `redis-cli` installed, install the plugin using `heroku`:

```console
$ heroku plugins:install https://github.com/stvp/heroku-redisgreen.git
```

### Usage

This client plugin supports both interactive mode and normal redis-cli use:

```console
$ heroku redisgreen:cli -a my-app SET mykey "hello world"
OK
$ heroku redisgreen:cli -a my-app GET mykey
"hello world"
$ heroku redisgreen:cli -a my-app
redis smart-dandelion-4.redisgreen.net:11035>
```
