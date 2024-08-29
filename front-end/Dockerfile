# Utilise la dernière version de nginx comme base
FROM nginx:latest

# Copier les fichiers du front-end dans le répertoire approprié de Nginx
COPY ./ /var/www/html/softy-pinko-front-end

# Copier le fichier de configuration Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

COPY ./favicon.ico /var/www/html/softy-pinko-front-end/favicon.ico

CMD ["nginx", "-g", "daemon off;"]
