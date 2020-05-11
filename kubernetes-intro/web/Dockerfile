FROM nginx

RUN mkdir /app
RUN echo "server { listen 8000 default_server; root /app; index index.html; }" > /etc/nginx/conf.d/default.conf
RUN useradd -u 1001 www
RUN sed -i 's/user  nginx/user www/g' /etc/nginx/nginx.conf;

EXPOSE 8000
