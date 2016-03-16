# Docker config for hthar.tk

Quick start: `docker-compose build && docker-compose up -d`

**Make sure to change the relay password!**

## HTTPS

[https-portal](https://github.com/SteveLTN/https-portal) provides an automatically configured nginx reverse proxy that uses Let's Encrypt certs.

## Weechat

A relay is started and can be connected to on port 443.

The password is empty by default; either change it in `weechat/.weechat/relay.conf` before build, or change it after connecting:

```
/set relay.network.password hunter2
```

It's possible to connect to the weechat console, too:

```
docker exec -it dockerdefault_weechat_1 tmux attach
```