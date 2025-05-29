# docker-step
Docker Fundamentals & Building Containers

✅ Install Docker di Windows/Mac/Linux.
// Install Package <br>
apt install python3 <br>
apt install docker.io <br>
apt install kubernetes <br>
apt intall vim //(optioal editor)


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
