# docker-shadowsocks


Build a tiny docker image (compressed ~ 16MB) for shadowsocks based on [alpine](https://alpinelinux.org/)
linux. The versions of this dockerfile follows shadowsocks [releases](https://github.com/shadowsocks/shadowsocks/releases).


## Usage
```
snap install docker
```

Pull the latest version from [docker hub](https://hub.docker.com/r/ggicci/shadowsocks/):

```
docker pull ggicci/shadowsocks
```

And run it with command:

```
docker run -d -p 10001:10001 ggicci/shadowsocks -s 0.0.0.0 -p 10001 -m aes-256-cfb -k ${your_password}
```
