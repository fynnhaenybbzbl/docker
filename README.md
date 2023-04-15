# Dokumentation

Wenn man dieses Programm startet, startet eine Webseite auf dem folgendem Link: http://localhost:3000/
Das ist die Start-Seite und dann gibt es verschiedene Unterseiten:
/karten
/waffen
/agenten

Dort findet man die verschiedenen Valorant Eigenschaften der jeweiligen Seiten.

Dockerfile: Diese Docker-Datei baut ein Image auf dem Node.js-Image mit lts-alpine-Version auf. Sie installiert alle Projekt-Abhängigkeiten, gibt den Port frei und startet das Projekt. Die Datei ist gut dokumentiert und kommentiert für eine einfache Wartbarkeit des Images.

index.js: Webseite in Java-Script aufgebaut.

devcontainer.json: In der Datei werden verschiedene Einstellungen angegeben, wie z.B. der Name des Containers, das Docker-Image, das verwendet werden soll, und welche Ports des Containers an den Host weitergeleitet werden sollen. Außerdem wird eine Post-Create-Command angegeben, das nach der Erstellung des Containers ausgeführt wird, in diesem Fall "npm install", um die Abhängigkeiten zu installieren.