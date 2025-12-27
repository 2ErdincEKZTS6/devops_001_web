# DevOps Hello World 001

### Hello 001 - Project

Bu benim ilk DevOps Projem.

### Docker'a terminalden login olmak için
<hr>

```
docker login -u KULLANICI_ADI -p PAROLA
```
---

### Docker Image oluştur 
Info: komut devops_001_web/ dizini içerisinde çalıştırılmalı !!
```
docker build buildx --build-arg JAR_FILE_target/devops_001_web-1.0.0.jar --tag KULLANICI_ADI/devops_001_web:v003 . 
```

### Docker Container oluştur & çalıştır
```
docker run -it -d -p DIŞ_PORT:8080 --name CONTAINER_ADI KULLANICI_ADI/devops_001_web:v003   
```
