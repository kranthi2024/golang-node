# Golang docker images with node

    Golang
    NodeJS
    Python

# Steps to push
-  docker login
-  docker build -t golang-node:1.24 .
-  docker tag golang-node:1.24 kranthivolt/golang-node:1.24
-  docker push kranthivolt/golang-node:1.24
