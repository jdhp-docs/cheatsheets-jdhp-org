
## Docker only

```
docker build -t cheatsheets-jdhp-org .
```

```
docker run -it -v $(pwd):/app -p 8080:8080 -d cheatsheets-jdhp-org npm install
```

```
docker run -it -v $(pwd):/app -p 8080:8080 -d cheatsheets-jdhp-org npm run
```

## Docker Compose


```
docker-compose up
```