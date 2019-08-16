
1) docker-compose up

2)    потом в новой вкладке 
      меняем домен и емейл  и запускаем 
docker run -it --rm -v init_https-certs:/etc/letsencrypt  --volumes-from webservertmp certbot/certbot certonly --webroot --webroot-path=/usr/share/nginx/html -d devbestlookmybet.tk -d www.devbestlookmybet.tk  --email  biryukwolf1@gmail.com  --agree-tos

3) останавливаем сервер  webservertmp

4) при желание можно запускать по крону 0 0 12 * * * 