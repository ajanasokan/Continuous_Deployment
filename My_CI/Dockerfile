FROM nginx:alpine

ARG BUILD_NUMBER
ARG IMAGE_NAME

COPY index.html /usr/share/nginx/html/index.html

RUN sed -i 's|{{BUILD_NUMBER}}|'${BUILD_NUMBER}'|g' /usr/share/nginx/html/index.html && \
    sed -i 's|{{IMAGE_NAME}}|'${IMAGE_NAME}'|g' /usr/share/nginx/html/index.html
