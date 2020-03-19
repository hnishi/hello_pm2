# hello_pm2

playground of pm2

```
docker build -f Dockerfile.dev -t hnishi/hello_react_node:dev .
docker run -v ${PWD}:/app -v /app/client/node_modules -v /app/server/node_modules -p 4000:4000 -p 3000:3000 --rm hnishi/hello_react_node:dev
```

## References

- [PM2 - Docker Integration](https://pm2.keymetrics.io/docs/usage/docker-pm2-nodejs/)
- [Run multiple services in a container](https://docs.docker.com/config/containers/multi-service_container/)

