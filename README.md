Symfony Docker deployment exemple

Pour reproduire ce déploiement dans votre projet Symfony :
1. Créer un dossier docker avec les fichiers suivant :

- apache.conf
- entrypoint.sh

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

6. Se connecter au serveur distant et déployer le projet
```bash
docker compose up
```

