# Redis Sentinel in Docker

## Run
```bash
docker compose up -d
```

## Stop Master
```bash
docker stop redis-master
```

## Check Master
```bash
docker exec -it sentinel-1 redis-cli -p 26379
redis-cli > SENTINEL get-master-addr-by-name mymaster
...
```