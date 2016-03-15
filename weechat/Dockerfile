FROM gliderlabs/alpine:3.3

RUN apk-install weechat tmux
ADD .weechat /root/.weechat
EXPOSE 9001

ENTRYPOINT ["tmux", "new-session", "weechat"]