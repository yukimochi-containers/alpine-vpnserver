# SoftEther VPN - An Open-Source Free ​Cross-platform Multi-protocol VPN Program

Extremely small footprint vpnserver container.

## Usage (sample)

````
mkdir -p /home/yukimochi/vpnserver/logs
cd /home/yukimochi/vpnserver/logs
mkdir packet_log security_log server_log
docker run -d -v /home/yukimochi/vpnserver/vpn_server.config:/usr/vpnserver/vpn_server.config  -v /home/yukimochi/vpnserver/logs:/usr/vpnserver/logs --net host --cap-add NET_ADMIN --name vpnserver yukimochi/alpine-vpnserver
````

## Supported architectures
[`amd64`](https://github.com/yukimochi-containers/alpine-vpnserver/blob/master/Dockerfile), [`arm32v7`](https://github.com/yukimochi-containers/alpine-vpnserver/blob/armv7/Dockerfile), `armhf`, [`arm64v8`](https://github.com/yukimochi-containers/alpine-vpnserver/blob/master/Dockerfile.aarch64)
