# test_enrollment
#Description
Il s'agit d'une injecton SQL sur une plateforme d'enregistrement; en clair sur un login page.
#Titre de l'exploit
Projet de système d'inscription v1.0 - Contournement de l'authentification par injection SQL (SQLI) et en anglais "Enrollment System Project v1.0 - SQL Injection Authentication Bypass (SQLI)".
#Lien de téléchargement du code source
https://www.sourcecodester.com/php/14444/enrollment-system-project-source-code-using-phpmysql.html
#CVE relatif
CVE-2023-33584
#Objectif
Cette vulnérabilité permet à un pirate de manipuler les requêtes SQL exécutées par l'application. Le système ne valide pas correctement les données fournies par l'utilisateur dans les champs nom d'utilisateur et mot de passe pendant le processus de connexion, ce qui permet à un pirate d'injecter du code SQL malveillant. En exploitant cette vulnérabilité, un pirate peut contourner l'authentification et obtenir un accès non autorisé au système.
#Lien pour lancer la page
Après avoir télécharger le fichier compressé, il faut le dézipper et le mettre dans le dossier www(sur wamp) ou htdoc(sur xamp) puis dans le navigateur, copier l'adresse suivante http://localhost/enrollment/login.php
#Action à effectuer une fois sur la page
Dans les champs nom d'utilisateur et mot de passe, insérez la charge utile d'injection SQL suivante, indiquée entre parenthèses, pour contourner l'authentification : {' ou 1=1 #}.
![Enrollement](https://github.com/akarrel/test_enrollment/assets/54906842/def7fecb-5c2d-498d-aaf5-9881942e7959)
#Commentaire
Après avoir suivi toutes les étapes, l'injection SQL n'a pas fonctionné comme le montre l'image ci-dessus.
Merci.
