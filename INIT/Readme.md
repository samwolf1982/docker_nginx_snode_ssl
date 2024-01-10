
1) docker-compose up

2) потім в новій вкладці замінити домен та пошту і запустити

docker run -it --rm -v init_https-certs:/etc/letsencrypt  --volumes-from webservertmp certbot/certbot certonly --webroot --webroot-path=/usr/share/nginx/html -d devbestlookmybet.tk -d www.devbestlookmybet.tk  --email  biryukwolf1@gmail.com  --agree-tos

3) зупинити сервер  webservertmp

4) якщо використовувати крон 0 0 12 * * * 
