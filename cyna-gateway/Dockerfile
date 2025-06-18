FROM node:20

# Dossier de travail dans le conteneur
WORKDIR /app

# Copie des fichiers de dépendances
COPY package*.json ./

# Installation des dépendances
RUN npm install

# Copie du reste du code source
COPY . .

# Port exposé (optionnel ici mais utile pour documentation)
EXPOSE 2000

# Commande de démarrage (mode dev si ts-node-dev)
CMD ["npm", "run", "dev"]