# cp

> Kopiere Dateien und Verzeichnisse.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/manual/html_node/cp-invocation.html>.

- Kopiere eine Datei an einen anderen Ort:

`cp {{pfad/zu/ausgangs_datei.ext}} {{pfad/zu/ziel_datei.ext}}`

- Kopiere eine Datei in ein anderes Verzeichnis und behalte den Dateinamen bei:

`cp {{pfad/zu/ausgang_datei.ext}} {{pfad/zu/ziel_verzeichnis}}`

- Kopiere die Inhalte eines Verzeichnisses rekursiv zu einem neuen Ort (wenn das Ziel existiert, wird das Verzeichnis ins bestehende Ziel Verzeichnis kopiert):

`cp {{[-r|--recursive]}} {{pfad/zu/ausgangs_verzeichnis}} {{pfad/zu/ziel_verzeichnis}}`

- Kopiere ein Verzeichnis rekursiv im ausführlichen Modus (zeigt die Dateien die kopiert werden):

`cp {{[-vr|--verbose --recursive]}} {{pfad/zu/ausgangs_verzeichnis}} {{pfad/zu/ziel_verzeichnis}}`

- Kopiere text Dateien zu einem anderen Ort im interaktiven Modus (fragt die Nutzer:in bevor eine Datei überschrieben wird):

`cp {{[-i|--interactive]}} {{*.txt}} {{pfad/zu/ziel_verzeichnis}}`

- Folge symbolischen Verzeichnislinks vorm Kopieren:

`cp {{[-L|--dereference]}} {{link}} {{pfad/zu/ziel_verzeichnis}}`

- Benutze den vollen Pfad der Ausgangsdateien und erstelle alle fehlenden Verzeichnisse beim Kopieren:

`cp --parents {{quelle/pfad/zu/datei}} {{pfad/zu/ziel_datei}}`
