## Usage

```bash
git clone https://github.com/cnzgray/aria2-ariang-docker \
    && cd aria2-ariang-docker
    && docker build -rm -f Dockerfile -t aria2-ariang-docker:latest aria2
    && docker build -rm -f Dockerfile -t webdav:latest webdav

docker-compose up -d
```