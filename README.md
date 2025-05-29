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
  mkdir simple-app
  cd simple-app
  vim Dockerfile
```
FROM python:3.10
WORKDIR /app
COPY . .
RUN pip install flask
CMD ["python", "app.py"]
```
