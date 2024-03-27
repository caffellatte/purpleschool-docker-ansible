# 4-nginx-image

Execute commands in the `4-nginx-image` directory

## Create image `4-nginx-image`

```bash
docker build -t 4-nginx-image -f Dockerfile .
```

## Run container `4-nginx`

```bash
docker run --name 4-nginx -d 4-nginx-image
```

## Get into `4-nginx` container shell

```bash
docker exec -it 4-nginx bash
```

## Test

```bash
curl http://127.0.0.1:80
```

## Exit

```bash
exit
```

## Remove `4-nginx` container

```bash
docker rm -f 4-nginx
```

## Remove `4-nginx-image` iamge

```bash
docker image rm 4-nginx-image
```
