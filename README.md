# docker-starter

## Deploy
```
docker stack deploy -c docker-compose.yml <my app name>
```

## Stop
```
docker stack rm <my app name>
```

## Note
Because ports "80:80" is [not working on Windows](https://github.com/moby/moby/issues/33902), so we disable routing mesh
=> load balancer is not working on `web` service
