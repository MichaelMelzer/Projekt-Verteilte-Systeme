# Projekt-Verteilte-Systeme
Ein Projekt im Rahmen des Moduls "Verteilte Systeme" an der Hochschule Darmstadt

## Überblick
Bei dem Modul "Verteilte Systeme" ging es darum, verschiedene Techiken und Protokolle kennen zu lernen, mit denen verschiedene Systeme miteinander verbunden werde können.
Um dies umzusetzen, sollte ein Smart Home Sytem umgesetzt werden:

## Simulation einer Umgebung
Da keine physikalischen Sensoren oder andere Geräte bereitgestellt werden konnten, mussten diese simuliert werden. 
Um dies zu ermöglichen, habe ich mich dazu entschieden einen zentralen Manager zu erstellen, welcher dann die ganzen simulierten Untersysteme auf eigenen Threads startet. Dadurch sind alle Systeme komplett voneinander abgeschottet, und teilen untereinander keine Informationen auf der Code-Ebene.
Die simulierten Sensoren basieren bewusst auf einem Interface ISensor. Dadurch kann eine implementation mit realen Sensoren einfach umgesetzt werden.
