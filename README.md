# GESTION DE BIBLIOTHEQUE EN C

## Authentification :

* Accès admin: user: admin@mail  password: admin
* Accès utilisateur: user:*jmk@email.net* password: *premier* ; 
	             user:*dani@mail* password: *dani*
		

## FONCTIONNEMENT DU PROGRAMME:

* l'utilisateur peut s'inscrit et se connecter pour emprunter un livre
* l'administrateur peut enregistrer des auteurs, des livres et administrer tout le systeme
* les statistiques presentées donnent un apperçu de l'etat du systeme

## CONFIGURATION:

* Importer la base de donnée contenu dans le dossier BD, dans MYSQL
* installer mysql client
#### 
    sudo apt-get install mysql-client
    sudo apt-get install libmysqlclient-dev

* Conpiler les fichiers
####
	make all
	gcc -o test $(mysql_config --cflags) main.c $(mysql_config --libs)
	
## LANCER LE PROGRAMME:
Se mettre dan le dossier *src* et executer la commande suivante
####
	./test
