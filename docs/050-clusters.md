# Clusters

Clusters, if applicable, are named with "docker names generator" utility.

Sample generator:

https://marc.codeberg.page/docker-name-generator/

Or just:

```
for i in $(seq 5); do docker run hello-world > /dev/null; done
docker ps -a --format '{{.Image}} {{.Names}}' | grep hello-world | cut -d' ' -f2 | sed 's/_/-/g'
```

Source of truth for allocated cluster names is this repository.

## Allocated names

```
brave-booth (@caramel, 2024)
funny-bell (@kitkat, 2026q1)
```

And some legacy ones:

```
dogseen
ufoo
```
