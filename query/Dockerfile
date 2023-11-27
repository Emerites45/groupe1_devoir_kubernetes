From node:alpine
  # Utilisez une image de base contenant Node.js
 

   # Définir le répertoire de travail dans le conteneur
 WORKDIR /Bureau/projet docker/tp-blog/query
 

   # Copier le package.json et package-lock.json dans le conteneur
COPY package*.json ./

   # Installer les dépendances du projet
   RUN npm install
   RUN apk update && apk add --no-cache curl

   # Copier tous les fichiers du projet dans le conteneur
   COPY . .

   # Exposer le port sur lequel l'application écoute
   EXPOSE 4002

   # Commande pour démarrer l'application
   CMD [ "npm", "start" ]
