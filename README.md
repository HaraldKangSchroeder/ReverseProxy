# HomeReverseProxy

## Build Image
docker build . -t <IMAGE_NAME>

## RUN IMAGE
 docker run --env-file ./.env -d <IMAGE_NAME>