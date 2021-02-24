# ctzndocker

A docker-compose to fire up new [CTZN](https://github.com/pfrazee/ctzn)'s server with Ngnix and Certbot

## Installation

1. Replace `example.com` with your domain in `entrypoint.sh`, `nginx.conf` and `docker-compose.yml`
2. Replace `example@gmail.com` with your email in `entrypoint.sh`
3. Run

```sh
docker-compose up -d
```

## Or docker run

```sh
docker run -e DOMAIN=localhost naoufalzerai/ctznserver 
```
