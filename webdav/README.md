# NGINX WebDAV container

Usage:

```bash
cd webdav && docker build --rm -f Dockerfile -t webdav:latest .

docker run --name webdav -d --restart always \
    -v /mnt/download:/media\
    -p 8000:80 \
    -e UID=$UID \
    webdav:latest
```

Optionally you can add two environment variables for basic authentication:

* WEBDAV_USERNAME
* WEBDAV_PASSWORD

