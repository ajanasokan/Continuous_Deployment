FROM nginx:alpine

ARG BUILD_NUMBER
ARG IMAGE_NAME

RUN echo "<h1>Ajan triggered the Jenkins pipeline</h1>" > /usr/share/nginx/html/index.html && \
    echo "<h2>Build Number: $BUILD_NUMBER</h2>" >> /usr/share/nginx/html/index.html && \
    echo "<h3>Docker Image: $IMAGE_NAME:build_number_$BUILD_NUMBER</h3>" >> /usr/share/nginx/html/index.html
