# Girlsday2024

Hallo zusammen,
der Girlsday ist vorbei und ihr seid hoffentlich heil mit eurem SmartMirror zuhause angekommen. Schaltet den Spiegel am besten dort ein, wo er auch am Ende stehen soll. Auf dem Raspberry Pi im dem SmartMirror läuft ein Betriebssystem, und dieses hat es nicht gern, wenn man den Strom einfach abschaltet ohne den Raspberry ordnungsgemäß herunterzufahren. 
Um den Raspberry zu konfigurieren oder auch auszuschalten, müsst ihr entweder eine Tastatur und Maus über einen [Micro USB Hub](https://amzn.eu/d/gOArXy9) an dem Pi anschließen, oder euch über ein [SSH Programm](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) (putty-64bit-0.81-installer.msi für aktuelle Windows Rechner) mit dem Raspberry verbinden. Ihr könnt euch jedoch nur mit dem Raspberry über einen Computer verbinden, wenn der MagicMirror sich auch erfolgreich in euer WLAN einloggen konnte. Startet der MagicMirror udn zeigt euch die korrekte Uhrzeit an, so sollte auch die Verbindung in euer WLAN in Ordnung sein. 
Klappt alles wie gewünscht könnt ihr euch jetzt mit der IP-Adresse des Spiegels und dem SSH Client mit dem Spiegel verbinden:

## Ein paar wichtige Daten:
Der Benutzername des Users auf dem Pi lautet "pi"
Der Ort, an welchem Ihr die Hauptkonfiration für den MagicMirror machen könnt, lautet: /home/pi/MagicMirror/config/config.js
Um diese Datei zu bearbeiten, müsst ihr in dem SSH Programm den Texteditor "nano" starten und diese Datei laden. Das macht ihr mit dem Befehl:
nano /home/pi/MagicMirror/config/config.js
Den Text einfach in eurem SSH Programm eingeben, und dann sollte sich die Datei öffnen. Hier könnt ihr jeztz mit den Pfeiltasten navigieren und zu der Stelle springen, an welcher Ihr was ändern möchtet. Um die Änderungen zu speichern, drückt bitte strg-o, dann wird gespeichert und mit strg+x wird das Programm nano wieder beendet. Die "strg" Taste findet ihr vermutlich ganz unten links auf eurer Tastatur. Dann einfach diese Taste gedrückt halten, und die Taste "o" oder "x" zusätzlich drücken.

### Installtionsart
Hier ist die offizielle Projektseite des [MagicMirrors](https://docs.magicmirror.builders/) 
Leider unterstützt diese Softwareversion den von uns verwendeten Raspberry Pi Zero nicht. Daher habe ich ein neues raspbian (das reguläre Betriebssystem des Raspberrys) installiert, noch keine updates eingespielt und dann dieses [Installationsscript](https://github.com/sdetweil/MagicMirror_scripts) ausgeführt.



