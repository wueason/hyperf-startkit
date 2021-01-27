English | [中文](./README-CN.md)

# Introductions

An alternative way to explore and develop with `[Hyperf](https://github.com/hyperf/hyperf)`.

# Requirements

 - `Docker`
 - `docker-compose`

# Usage

- Generate Docker image `docker-compose build`
- Install `composer.json` dependencies `docker-compose run --rm hyperf-web "composer install --no-dev"`
- Start service `docker-compose up -d`
- Visite: usually `http://192.168.99.100:9501` on `Windows`, `http://127.0.0.1:9501` on `Linux`/`Mac`

# Tips

- On `Windows`, put your code in path `C:\Users\{USERANME}`, or docker volume mount will be failed
- When `Dockerfile` has a change, you need to rebuild docker image `docker-compose build`
