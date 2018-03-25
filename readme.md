# SoftEther VPN - An Open-Source Free ​Cross-platform Multi-protocol VPN Program

Extremely small footprint vpnserver container.

## Build status

### latest (Stable Edition)

- amd64 image - ![AMD64 Stable Edition image Build status](https://img.shields.io/docker/build/yukimochi/alpine-vpnserver.svg)
- arm32v7 image - ![arm32v7 Stable Edition image Build status](https://ci.yukimochi.com/api/badges/yukimochi-containers/alpine-vpnserver/status.svg?branch=armv7)
- arm64v8 image - ![arm64v8 Stable Edition image Build status](https://ci.yukimochi.com/api/badges/yukimochi-containers/alpine-vpnserver/status.svg?branch=master)

### edge (Developer Edition)

- amd64 image - ![AMD64 Developer Edition image Build status](https://img.shields.io/docker/build/yukimochi/alpine-vpnserver.svg)
- arm32v7 image - ![arm32v7 Developer Edition image Build status](https://ci.yukimochi.com/api/badges/yukimochi-containers/alpine-vpnserver/status.svg?branch=edge-armv7)
- arm64v8 image - ![arm64v8 Developer Edition image Build status](https://ci.yukimochi.com/api/badges/yukimochi-containers/alpine-vpnserver/status.svg?branch=edge)

## Usage (sample)

````
mkdir -p /home/yukimochi/vpnserver/logs
cd /home/yukimochi/vpnserver/logs
mkdir packet_log security_log server_log
docker run -d -v /home/yukimochi/vpnserver/vpn_server.config:/usr/vpnserver/vpn_server.config  -v /home/yukimochi/vpnserver/logs:/usr/vpnserver/logs --net host --cap-add NET_ADMIN --name vpnserver yukimochi/alpine-vpnserver
````

## Supported architectures
[`amd64`](https://github.com/yukimochi-containers/alpine-vpnserver/blob/master/Dockerfile), [`arm32v7`](https://github.com/yukimochi-containers/alpine-vpnserver/blob/armv7/Dockerfile), [`arm64v8`](https://github.com/yukimochi-containers/alpine-vpnserver/blob/master/Dockerfile.aarch64)
