# docker-shadowsocks-libev

[![](https://travis-ci.org/lostsnow/docker-shadowsocks-libev.svg)](https://travis-ci.org/lostsnow/docker-shadowsocks-libev)

Current version: [3.3.1][1]

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
curl -x socks5://<client-ip>:1080 https://www.google.com/
```

## Changelog

### 3.0.7

* add support for [simple-obfs][5] plugin
* add ARGS env variable

### 3.0.0

* deprecate OTA (One-Time-Auth)
* add support for [AEAD][4]


[1]: https://github.com/shadowsocks/shadowsocks-libev/releases
[2]: https://hub.docker.com/r/lostsnow/shadowsocks-libev/
[3]: https://github.com/lostsnow/docker-shadowsocks-libev/blob/master/docker-compose.yml
[4]: https://shadowsocks.org/en/spec/AEAD-Ciphers.html
[5]: https://github.com/shadowsocks/simple-obfs
