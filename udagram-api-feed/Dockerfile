FROM node:12

# Créer le répertoire de l'application
WORKDIR /usr/src/app

# Installer les dépendances de l'application
# Un joker est utilisé pour s'assurer que le package.json ET package-lock.json sont copiées lorsqu'ils sont disponibles
COPY package*.json ./
RUN npm install

# Regroupe des sources de l'application
COPY . .
EXPOSE 8080
CMD ["npm", "run", "prod"]

