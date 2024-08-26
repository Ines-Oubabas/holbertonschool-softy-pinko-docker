# Utilise la dernière version d'Ubuntu comme base
FROM ubuntu:latest

# Met à jour les listes de paquets APT et effectue une mise à jour complète
RUN apt-get update && apt-get upgrade -y

# Installe Python3 et pip3
RUN apt-get install -y python3 python3-pip

# Supprime le fichier EXTERNALLY-MANAGED si présent pour éviter les erreurs lors de l'installation des paquets Python
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Installe Flask via pip3
RUN pip3 install flask

# Définit le répertoire de travail dans le conteneur
WORKDIR /app

# Copie le fichier api.py dans le conteneur
COPY ./api.py /app/api.py

# Définit la commande pour démarrer l'application Flask
CMD ["python3", "api.py"]

