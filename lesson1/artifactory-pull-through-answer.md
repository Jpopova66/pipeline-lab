# Занятие 1. Шаг 6. Скачивание образа через Artifactory

Docker скачал образ через виртуальный Docker-репозиторий `docker`. Artifactory получил образ из GHCR через удалённый репозиторий `docker-ghcr` и сохранил копию в кэше. В интерфейсе JCR тег виден по пути `docker-ghcr-cache → jpopova66 → pipeline-lab → latest`.

В этом стенде используется метод Repository Path на опубликованном порту `8081`.

```text
docker pull localhost:8081/docker/jpopova66/pipeline-lab:latest
Digest: sha256:bfbf05bf10f389a878d36921183d54db31f7787f4389777e8b94c4df89e8fff1
Status: Downloaded newer image for localhost:8081/docker/jpopova66/pipeline-lab:latest
```
