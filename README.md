gibby/syncthing
===================
[![](https://images.microbadger.com/badges/image/gibby/syncthing.svg)](https://microbadger.com/images/gibby/syncthing "Get your own image badge on microbadger.com")


[Syncthing](http://syncthing.net/) Docker image

Forked from https://github.com/istepanov/docker-syncthing

### How to run

    docker run -d \
        --name syncthing \
        --restart always \
        -p 8384:8384 -p 22000:22000 -p 21025:21025/udp \
        -v /opt/docker/syncthing/config:/home/syncthing/.config/syncthing \
        -v /opt/docker/syncthing/Sync:/home/syncthing/Sync \
        gibby/syncthing

Then access Syncthing Web UI at [http://localhost:8384/]()
