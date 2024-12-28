```
mkdir windows-docker
```

```
vim compose
```

```
services:
  windows:
    image: dockurr/windows
    container_name: windows
    environment:
      VERSION: "11"
      RAM_SIZE: "8GB"
      CPU_CORES: "4"
      DISK_SIZE: "128"
    devices:
      - /dev/kvm
      - /dev/net/tun
    cap_add:
      - NET_ADMIN
    ports:
      - 8006:8006
      - 3389:3389/tcp
      - 3389:3389/udp
    stop_grace_period: 2m
    restart: on-failure
    volumes:
      - ./data:/storage/shared/```

```
```
sudo docker-compose
```
