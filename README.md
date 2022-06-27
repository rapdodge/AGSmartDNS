# AGSmartDNS
[Docker] AdGuard Home + SmartDNS

This repository makes it easy to create AdGuardHome and SmartDNS docker containers

## Quick Start

```shell
docker compose up -d
```

## Customization
You should have basic knowledge about docker-compose, Dockerfile, and SmartDNS configuration

docker-compose location is on the root of this repository

Dockerfile and smartdns.conf is on smartdns directory of this repository

## Networking
I'm using static IP for the containers

172.16.0.2 is for AdGuard Home

172.16.0.3 is for SmartDNS

## Basic Configuration
Open [ip]:3000 on browser, and do the setup, for really basic configuration, change admin web interface, you should change it from 80 to 3000, or if you want to customize it, you can edit docker-compose file and adding the port

![image](https://user-images.githubusercontent.com/33513626/175992548-7f8efd99-b531-4f41-854c-14f5fda07e67.png)

After that setup and logged in to the admin web interface, go to Settings -> DNS settings, change "Upstream DNS servers" to 172.16.0.3:6053

![image](https://user-images.githubusercontent.com/33513626/175993047-64403b94-d412-465e-a523-7d09e76c91d4.png)

And you ready to go! You can customize other settings that you like :)

## Special Thanks
[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) for making best network-wide ads & trackers blocking DNS server

[SmartDNS](https://github.com/pymumu/smartdns) to make DNS response as fast as possible
