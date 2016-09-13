# docker-shadowsocks-libev

[![](https://travis-ci.org/lostsnow/docker-shadowsocks-libev.svg)](https://travis-ci.org/lostsnow/docker-shadowsocks-libev)

Current version: [2.5.2][1]

## docker image

See [lostsnow/shadowsocks-libev][2]

## Usage

change some environment variables in [docker-compose.yml][3].

```bash
# server
docker-compose up -d server

# client
docker-compose up -d client

# usage
curl -x socks5h://<client-ip>:1080 https://www.google.com/
```

[1]: https://github.com/shadowsocks/shadowsocks-libev/releases
[2]: https://hub.docker.com/r/lostsnow/shadowsocks-libev/
[3]: https://github.com/lostsnow/docker-shadowsocks-libev/blob/master/docker-compose.yml
