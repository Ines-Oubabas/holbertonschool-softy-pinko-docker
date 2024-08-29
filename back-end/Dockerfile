# Use the latest Ubuntu image
FROM ubuntu:latest

# Update and upgrade APT packages
RUN apt-get update && apt-get upgrade -y

# Installer Python3 et pip3
RUN apt-get install -y python3 python3-pip

# Résoudre le problème de l'environnement géré
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Installer Flask avec pip3
RUN pip3 install flask

# Installer Flask et flask-cors avec pip3
RUN pip3 install flask flask-cors

# Définir le répertoire de travail à /app
WORKDIR /app

# Copier le fichier api.py dans le conteneur
COPY api.py /app/api.py

# Exposer le port 5252
EXPOSE 5252

# Commande pour exécuter l'application Flask
CMD ["python3", "api.py"]
