# docker-step
Docker Fundamentals & Building Containers

✅ Install Docker di Windows/Mac/Linux.
```
// Install Package
apt install python3
apt install docker.io
apt install kubernetes
apt intall vim //(optioal editor)
```

✅ Build dan Run Aplikasi Sederhana:
● Buat folder simple-app/.
```
mkdir simple-app
cd simple-app
```
Write Dockerfile with vim
```
  vim Dockerfile
```

Isian dari Dockerfile
```
FROM python:3.10
WORKDIR /app
COPY . .
RUN pip install flask
CMD ["python", "app.py"]
```


✅ Build & Run Image:
```
docker build -t simple-app:v1 .
docker run -d -p 5000:5000 simple-app:v1
```
docker run akan menampilak container_id


(opional) see running logs
```
docker logs <container_id>
```

✅ (Optional Challenge): Push ke Docker Hub
```
docker build -t <yourusername>/<yourimagename>:<tag> .
```

sample:
```
docker build -t kitatech/simple-app:latest .
```

<img src="images.png">

then push to Docker HUB
```
docker push kitatech/simple-app:latest
```
