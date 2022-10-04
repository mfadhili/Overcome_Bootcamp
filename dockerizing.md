Dockerize app:
    FROM nginx:alpine
    COPY . /usr/share/nginx/html .

Build the docker image
    docker build -t <image-name:v1> .
    example: docker build -t natujenge-oyf-group3:v1 .

Run the container
    docker run -d -p 8080:80 natujenge-oyf-group3:v1

Confirm it's running
    curl localhost:8080