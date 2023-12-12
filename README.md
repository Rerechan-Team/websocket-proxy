# websocket

没什么技术含量就是SSH -D 加强版,只是方便我自己使用，用过其他第三方的都不支持轮询.就自己撸了一个。,可以根据请求的IP归属地、域名、域名解析IP归属地 进行路由。
配置文件支持多vps，单vps多端口，自己轮询。,ssh转发代理，服务器不需要安装任何服务端。 设置好配置信息后，浏览器或wifi设置中可以设置SOCKS5代理, 建议通过下面命令创建一个只允许 TCP 转发而不允许登陆（交互）的 SSH 账号。


```
config.yml:
verbose: 0
listen:
- target_host: 127.0.0.1
  target_port: 22
  listen_port: 8880
```

2. Run websocket.
```
ws-enhanced -f config.yml
```