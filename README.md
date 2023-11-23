# Stats-tests_de_normalit-s-
#Créer un environnement de travail et installer les dépendances
virtualenv .venv
.venv\\Scripts\\activate 
pip install -r requirements.txt

#Créer une data base
#Créer une base de donnée PGSQL et entrer les informations dans un fichier .env a la racine du projet

DATABASE_NAME=<your_database_name>
DATABASE_PWD=<your_database_password>
DATABASE_USER=<your_database_user>

#Executer les migrations Django
#Pour créer les tables dans la base de donnée, il faut executer les migrations.

#Créer les migrations
py manage.py makemigrations

#Effectuer les migrations
py manage.py migrate

#Run
py manage.py runserver

