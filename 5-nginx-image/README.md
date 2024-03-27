# 5-nginx-image

Execute commands in the `5-nginx-image` directory

## Create image `5-nginx-image`

```bash
docker build -t 5-nginx-image -f Dockerfile .
```

## Run container `5-nginx`

```bash
docker run --name 5-nginx -d -p 8081:80 5-nginx-image
```

## Test

```bash
curl http://127.0.0.1:8081
```

## Remove `5-nginx` container

```bash
docker rm -f 5-nginx
```

## Remove `5-nginx-image` iamge

```bash
docker image rm 5-nginx-image
```
