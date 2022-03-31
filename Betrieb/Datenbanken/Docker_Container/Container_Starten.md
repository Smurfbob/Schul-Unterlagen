# Starten eines Docker Containers

+ Zuerst muss das Tool Rancher Desktop gestartet werden
+ Danach nutzt man eine .yml Datei, welche Informationen für den Container bereitstellt
+ Im letzten Schritt, muss der folgende Befehl auf die Datei ausgeführt werden
``` 
docker-compose -f  .\fileName.yml up
```
+ Danach sollte der Container starten