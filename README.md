# Mozilla Firefox

Rode o Mozilla Firefox dentro de um container docker.


#### Como testar?

```
docker run -it --rm --net=host --env="DISPLAY" \
           --cpuset-cpus 0 --memory 512mb \
           --volume="$HOME/.Xauthority:/root/.Xauthority:rw" \
           --volume="$HOME/Firefox-Container/Downloads:/root/Downloads:rw" \
           seniocaires/mozilla-firefox
```
