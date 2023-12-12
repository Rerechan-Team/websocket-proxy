# websocket http

该代理将为 ssh websocket http 修复负载增强协议创建代理服务器

config.yml
```
verbose: 0
listen:
- target_host: 127.0.0.1
  target_port: 22 # 这是 openssh 的端口，将用作下一个端口的目的地
  listen_port: 8880 # 这是 websocket http 8880 协议的端口，它将在目标端口上转发
```

2. Run websocket.
```
ws-enhanced -f config.yml
```
# Untest Version @Rerechan02
