# LeProjet

### Première installation ###

Tout d'abord, il faut installer un client Git. Pour avoir plus de contrôle, on peut utiliser la console Git: https://git-scm.com/download/

Lors de l'installation, utilisez les options par défaut. Une fois que c'est installé, démarrez le programme Git Bash. Vous allez vous retrouver sur une fenêtre en ligne de commande qui fonctionne de la même manière que sur Linux:

![](http://i.imgur.com/9SSrbD9.png)

Allez au dossier où vous voulez installer le projet avec la commande `cd`. Dans mon cas, `cd /d/Projects/UnrealEngine/`.
Lorsque vous faites la commande `ls`, il est possible de voir tous les dossiers et fichiers à l'intérieur du répertoire courrant.
Par défaut, le répertoire courrant est dans le C:\Utilisateurs\NomUtilisateur.

Pour installer le projet, `git clone https://github.com/samuellapointe/LeProjet.git`

Le projet est maintenant disponible dans ce dossier, vous pouvez double-cliquer sur le ficher LeProjet.uproject pour le démarrer. 
### Effectuer des changements ###

Je viens de créer un matériel nommé MetalBleu, je l'ai appliqué à un cube et j'ai reconstruit (build) la scène. Il est maintenant temps de rendre les changements disponibles pour tout le monde. Dans la console Git, entrez dans le dossier du projet avec `cd`. Dans ce dossier, faites `git status` pour voir la liste des fichier créés et modifiés:

![](http://i.imgur.com/GL6N25Q.png)

Pour choisir les fichiers à envoyer, faites `git add fichier`. Pour envoyer toutes les modifications, `git add .` Ensuite, `git commit -m "message"` où message est un message pertinent explicant les modifications.

Le commit est sur votre ordinateur local. Pour le partagez avec tout le monde, il faut d'abord aller chercher la dernière version du projet, au cas où des modifications aurait eu lieu. Pour ce faire, `git pull --rebase`.

Il se pourrait qu'il y ait des conflits à cette étape, par exemple si quelqu'un a modifié la même image que vous. Dans ces situations, il faut déterminer quelle version de l'image garder. Dans le cas des fichiers textes comme le code, git n'aura habituellement pas de problème à intégrer vos modifications au fichier. En cas de problème, je pourrais vous aider.

Enfin, pour envoyer la modification, `git push`. Il faudra entrer votre nom d'utilisateur et mot de passe GitHub. Si vous n'avez pas été ajouté à la liste des contributeurs, il ne vous laissera pas ajouter la modification. Contactez moi ou un autre membre pour qu'on vous rajoute.

### En résumé ###
    git add .
    git commit -m "lol"
    git pull --rebase
    git push
