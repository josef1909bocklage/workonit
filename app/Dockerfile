FROM nginx:1.19-alpine

WORKDIR /app

COPY . .

COPY nginx/nginx.conf /etc/nginx/conf.d/default.conf
COPY html/ /usr/share/nginx/html
RUN chmod -R 770 /var/cache/nginx /var/run /var/log/nginx

EXPOSE 8081