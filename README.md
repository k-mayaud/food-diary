- Avoir installé php 8 avec ses dépendances
- Installer composer
- Lancer un composer install après avoir récupéré le projet ```composer install```
- Installer driver sqlite3 ubuntu ```sudo apt install php8.0-sqlite3 ```
- Installer la base de données 
  - ```php bin/console doctrine:database:create --env=test```
  - ```php bin/console doctrine:schema:create --env=test```
  - ```php bin/console doctrine:migrations:migrate --env=test```
- Changer dans le ```.env``` les valeurs suivantes que vous récupérez depuis Github(https://github.com/settings/apps)
  - GITHUB_ID
  - GITHUB_SECRET
- ```yarn install``` Pour générer les assets css et js via encore
- ```yarn dev``` Pour regénérer les assets automatiquement
- ```symfony server:start```

__Ne pas oublier de changer dans le fichier ```tests/Controller/DiaryControllerTest.php:21``` l'adresse mail, 
qui doit être celle utilisée sur Github__