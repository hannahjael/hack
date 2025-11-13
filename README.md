FROM nginx
COPY index.html /usr/share/nginx/html/index.html

docker build -t myapp .
docker run -d -p 8080:80 myapp .
