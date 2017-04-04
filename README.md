# Play Framework docker images

* [https://www.playframework.com/](https://www.playframework.com/)

## Play versions

### 1.2 
Play 1.2.5.6 [https://downloads.typesafe.com/play/1.2.5.6/play-1.2.5.6.zip](https://downloads.typesafe.com/play/1.2.5.6/play-1.2.5.6.zip)

Installation path `/play-1.2.5.6`

## Run app

```
docker run -d \
  -v /path/to/your/play/app:/app \
  -p 9000:9000 \
  alteom/playframework:1.2
```

## Play modules

```
docker run -d \
  -v /path/to/your/play/app:/app \
  -v /path/to/your/modules:/modules \
  -p 9000:9000 \
  alteom/playframework:1.2
```