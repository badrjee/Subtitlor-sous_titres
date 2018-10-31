# Subtitlor-sous-titres

Une application JEE qui permet de créer des fichiers de sous titres qu'ont peut utiliser dans des vidéos

Fonctionnalités :

- les fichiers générer sont au format .srt

- Utilisation du pattern DAO

- Enregistrement des fichiers .srt en base de données ainsi que leur traduction

- Export de fichiers .srt

- Upload de nouveau fichier à traduire

- Sélection d'un fichier à traduire ou chargement du dernier fichier édité

Exemple:

A partir d'un fichier "sous_titre.srt" avec le contenu écrit en "FR"on va crée un fichier "sous_titre_new.srt" avec le contenue traduit en "EN"; et pour cela on doit avoir le fichier de données "sous_titre.srt"

Execution du projet:

- Crée une base de donnée "subtitlor", Username="root", Password=""

- Utiliser le fichier Subtitlor.sql pour crée 2 tables "original" et "trasnlated"

- Déployer l'application sur votre serveur tomcat sur l'url : http://localhost:8080/Subtitlor/home

Remarque:

Avant de lancer l'application assurez que :

  - votre serveur utilise le bon port http (dans mon cas "8080")

  - ouvrir "web.xml" et modifier le chemin de votre fichier de données "sous_titre.srt" dans la balise "location",dans ce cas le fichier "sous_titre.srt" ce trouve dans le dossir: C:/Users/Badrjee/Desktop/FileData
