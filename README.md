Symfony Docker deployment exemple

Pour reproduire ce déploiement dans votre projet Symfony :
1. Créer un dossier docker avec les fichiers suivant :

- apache.conf
- entrypoint.sh

2. Créer un fichier Dockerfile

3. Créer un fichier compose.yaml

4. Créer une image de votre projet
```bash
docker build . -t symfony-example-deployment
```

5. Déployer le projet
```bash
docker compose up
```

