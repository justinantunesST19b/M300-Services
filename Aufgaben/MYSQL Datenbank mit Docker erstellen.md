# Aufgabe: MYSQL Datenbank mit Docker erstellen

Aus https://hub.docker.com/r/ubuntu/mysql den Command herausgesucht:

        docker run -d --name mysql-container -e -p 3306:3306 -e MYSQL_ROOT_PASSWORD=My:S3cr3t/ ubuntu/mysql:8.0-22.04_beta

Mit diesem Kommand erstellt man den Container:

Docker run -d

Den Namen gibt man an mit:

--Name "Name eingeben"

Den Portforwar erstellt man mit dem Kommand:
        -p 3306:3306
Die Linke Nummer darf varieren. Diese ist die Port die die VM besitzt.
Die rechte Nummer muss 3306 sein, da diese den Port angibt auf welcher man auf den Container zugreifen kann.

Das root Passwort gibt man an mit:
MYSQL_ROOT_PASSWORD="Passwort"

Den Tag gibt man mit dem Kommand:
ubuntu/mysql:8.0-22


Nachdem man eine Datenbank im MySQL Workbench erstellt hat, kann man mit diesen Commands auf das Verzeichnis in welchem die Datenbanken drinnen sind anschauen:

        docker exec -it 7c49f35071e1 /bin/bash 
--> auf docker verbinden und die Docker ID angeben

        cd /var/lib/mysql

        ls

Falls hier die Datenbank angezeigt wird, hat es funktioniert.       
