# Spy-s-partitions

#Sujet:

#Le but est de fabriquer un outil à base de shell-scripts Bourne pour surveiller le remplissage des différentes partitions d'un système.


#1)Créer un shell-script,sh1, qui soit tel que:
#	- Il fixe automatiquement la liste des partitions à surveiller (à partir de la commande df par exemple),
#	- il initialise un fichier log spécifique dans /var/log,
#	- il possède une fonction qui lui permette de déposer un message dans le fichier log avec, à chaque fois, la date et l'heure en début de ligne,
#	- il enregistre dans le fichier log le début de la surveillance,
#	- il execute une boucle infinie avec une pose de 5 minutes (réglable) entre chaque tour,
#	- à chaque tour de boucle il teste chaque partition et envoie un message si l'espace libre  est inférieur à 10% de l'espace total (réglable),
#	- il stoppe sur réception d'un signal SIGTERM avec un message dans le log.

#2) Créer un script s 2 qui fasse en sorte:
# - d'afficher le contenu du fichier log,
# - de réinitialiser le contenu du fichier log
# - d'indiquer si le service est actif ou pas

