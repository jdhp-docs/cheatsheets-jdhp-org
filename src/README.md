
## Docker only

```
docker build -t cheatsheets-jdhp-org .
```

Install JS dependencies (bootstrap, sass, http-server)
```
docker run -it -v $(pwd):/app -p 8080:8080 --user $(id -u):$(id -g) cheatsheets-jdhp-org npm install
```

Preprocess (compile) CSS
```
docker run -it -v $(pwd):/app -p 8080:8080 --user $(id -u):$(id -g) cheatsheets-jdhp-org npm run sass
```

Launch http-server
```
docker run -it -v $(pwd):/app -p 8080:8080 --user $(id -u):$(id -g) cheatsheets-jdhp-org npm start
```

## Docker Compose


```
docker-compose up
```