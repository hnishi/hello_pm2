# hello_pm2

playground of pm2

```
docker build -f Dockerfile.dev -t hnishi/hello_react_node:dev .
docker run -v ${PWD}:/app -v /app/client/node_modules -v /app/server/node_modules -p 4000:4000 -p 3000:3000 --rm hnishi/hello_react_node:dev
```

## PM2 is not recommended to use in dev env

> pm2 is meant for production usage.
npm start in Create React App is meant only for development as mentioned in its output message.


> The command itself is in node_modules/.bin. npm adds it to PATH automatically inside scripts.
>
> So the full command you want to run is node_modules/.bin/react-scripts start. Although it would be better to just run npm start in the project folder.

[running pm2 with npm script &quot;react-scripts start&quot; · Issue #774 · facebook/create-react-app](https://github.com/facebook/create-react-app/issues/774)

## References

- [PM2 - Docker Integration](https://pm2.keymetrics.io/docs/usage/docker-pm2-nodejs/)
- [Run multiple services in a container](https://docs.docker.com/config/containers/multi-service_container/)

