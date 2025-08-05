Symfony Docker deployment exemple

Pour reproduire ce déploiement dans votre projet Symfony :
1. Créer un dossier docker avec le fichier suivant :
- apache.conf

2. Créer un fichier Dockerfile

3. Créer un fichier compose.yaml

4. Créer une image de votre projet
```bash
docker build . -t symfony-deployment-example
```

5. Héberger l'image sur dockerhub
```bash
docker login
docker tag symfony-deployment-example <nom_utilisateur_dockerhub>/symfony-deployment-example
docker push <nom_utilisateur_dockerhub>/symfony-deployment-example
```

Adapter le projet avec votre version de PHP

Projet minimum avec :
- User entity
- Register & login