Methode avec SH LES etapes a suivre..............
creer un fichier Orcherstrateur.sh pour les données avec crumbtable a la racine du project 
creer run.sh dans scala
********************************************************************************************

stockage de API en local et sur HDFS (Orcherstrateur.sh)

données les droits sur mon dossier bigdata : chmod -R 777 ./

***************************************************************
injection.py pour recuperer API  et stockage sur hdfs et en local 
- creer un dossier Datalake sur hadoop 
-données les droit sur le fichier : hdfs dfs -chmod 777 /user/Datalake2/   **2eme commande **  hdfs dfs -chown ubuntu:ubuntu /user/Datalake2/

************************************************
Orcherstrateur.sh donneés les droit sur hdfs en ligne de commande
creation des dossier : hdfs dfs -mkdir -p /chemin du fichier
                       hdfs dfs -ls -R /
                       hdfs dfs -chmod -R 777 /chemin vers le fichier

********************************************************
configurer crontab 
sudo crontab -e
apres selectionné 1 
ajoute sa a la fin         0 * * * * sh /home/ubuntu/mnmcount/Orchestrateur.sh

afficher le contenue crontab -l
**********************************************
                    
                    