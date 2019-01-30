# Mozilla Firefox

Rode o Mozilla Firefox dentro de um container docker.


#### Como testar?

```
docker run -d --name=firefox --restart=always \
           --net=host --env="DISPLAY" \
           --cpuset-cpus 0 --memory 512mb \
           --volume="$HOME/.Xauthority:/root/.Xauthority:rw" \
           --volume="$HOME/Firefox-Container/Downloads:/root/Downloads:rw" \
           --volume="$HOME/Firefox-Container/data:/root/.mozilla:rw" \
           seniocaires/mozilla-firefox
```
