# loopback_container
docker loopback container image

## build
```
  docker build -t loopback:ffmpeg .
```
## use 
```
  docker run -d \
  -p 3000:3000 \
  -e PORT=3000 \
  -e NODE_ENV=production \
  -v /mnt/media_storage:/mnt/media_storage \
  -v /root/package:/package \
  --name=media-api-beta \
  loopback:ffmpeg
```
