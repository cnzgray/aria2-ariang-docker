## Usage

```
cd aria2 && docker build --rm -f Dockerfile -t aria2-ariang-docker:latest .

docker volume create aria2-conf
docker run --name ariang -d --restart always \
    -v /mnt/download:/data \
    -v aria2-conf:/root/conf \
    -p 6800:6800 -p 80:80 -p 443:443 \
    aria2-ariang-docker:latest

```