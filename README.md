# thingsboard_edge_compose

ThingsBoard的边缘计算节点的docker compose配置
> 参考文档：https://thingsboard.io/docs/user-guide/install/edge/docker/

## 配置.env

`CLOUD_ROUTING_KEY` 和 `CLOUD_ROUTING_SECRET`这两个变量在管理面板中可以找到
- 边缘管理 -> 边缘实例 -> 增加边缘 -> 边缘键/边缘密钥

`CLOUD_RPC_HOST`: 主机的ip地址

## 端口

- 8080: HTTP
- 1883: MQTT
- 5683-5688: UDP

## 注意

- Edge通过RPC协议连接到Server`7070`端口，确保防火墙允许通过