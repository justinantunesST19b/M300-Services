# Einfache Web-App in einen Container  verfrachten

## Vorbereitung

        $ mkdir TEMP_Docker  
Unterverzeichnis "TEMP_Docker" erstellen

        $ cd TEMP_Docker
Ins Unterverzeichnis "TEMP_Docker" wechseln 

        $ git clone https://gitlab.com/ser-cal/Container-CAL-webapp_v1.git   
Repo klonen

        $ cd Container-CAL-webapp-v1/  
Ins Repo-Unterverzeichnis hüpfen

        $ cd APP   
Ins Unterverzeichnis "APP" hüpfen 

        $ less Dockerfile 
Inhalt des Dockerfiles anschauen

        $ docker --version  
Nochmals sicherstellen, dass Docker installiert ist (Notwendig)

## Neues Docker-Image bauen

        $ docker image build -t justin5436/webapp_one:1.0 .
Erstelle ein neues Image in diesem Verzeichnis


## Neues Docker-Image überprüfen

        $ docker image ls  
Überprüfen, ob Image vorhanden ist

## Registrieren auf Docker-Hub