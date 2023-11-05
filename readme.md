# LB 324

## Aufgabe 2
Erklären Sie hier, wie man `pre-commit` installiert:

Zuerst erstellt man ein neues Terminal, um den Befehl "pip install pre-commit" einzugeben.
Somit wird ein File mit den Namen "pre-commit-config.yaml" erstellt.
Mit diesem File kann man zudem Sachen hinzufügen, wie das automatische Formatieren des Codes oder das automatische Ausführen von Tests.

## Aufgabe 4
Erklären Sie hier, wie Sie das Passwort aus Ihrer lokalen `.env` auf Azure übertragen:

Da ich das Projekt nicht auf Azure bringen konnte, da es nicht funktioniert hat, habe ich es dockerisiert.

Zuerst habe ich ein Dockerfile erstellt, dass Docker weiss, wie das Image zu erstellen ist. Um ein Image zu erstellen, habe ich ein neues Terminal erstellt und den Befehl "docker build -t freylukaslb-324 ." eingegeben. Nachdem das Image erstellt wurde, habe ich mit dem Befehl "docker run -d -p 5000:5000 freylukaslb-324" einen Container erstellen und laufen lassen. Um schlussendlich das Image auf DockerHub zu pushen, habe ich das Image mit dem Befehl "docker tag freylukaslb-324 freylukas/freylukaslb-324:tag" getagged. Damit das Image jetzt auf DockerHub gepushed wird, habe ich in der Dockerapp die zur Verfügung gestellte Funktion benutzt. Es gibt nähmlich in der App einen Button, mit dem man das Image auf DockerHub pushen kann.

Hier wäre der Link zu meinem Image auf DockerHub: https://hub.docker.com/repository/docker/freylukas/freylukaslb-324/general
