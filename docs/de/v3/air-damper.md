# Montage und Überprüfung der Belüftungsdrossel

## Anpassung
Vor der Installation des Servomotors im Drosselgehäuse muss das Gehäuse ohne ihn montiert und die Gängigkeit der Drossel überprüft werden. Die Drossel muss sich frei bewegen, ohne in irgendeiner Position zu verkleben. Bei Bedarf ist eine kleinere mechanische Überarbeitung der Drosselteile erforderlich (z. B. Grate entfernen, Sitze anpassen oder die Achse polieren).

## Installation auf die Welle
Nach Überprüfung der Gängigkeit können Sie die Drossel auf die Servo-Welle aufsetzen. Eine Befestigung mit einer Schraube ist nicht notwendig und kann in einigen Situationen sogar schädlich sein.

## Überprüfung vor der Montage
Überprüfung des Betriebs vor der Installation im Gehäuse
Es wird empfohlen, den Servomotor mit der Steuerplatine zu verbinden und die Funktionsprüfung der Baugruppe auf dem Tisch durchzuführen. Stellen Sie sicher, dass der Fensterladen bei Anwendung von Steuersignalen frei bewegt wird. Beseitigen Sie eventuelle Blockierungen vor dem Fortfahren mit der weiteren Montage.

Die Einstellung der Ausgangslage der Drossel erfolgt bei angeschlossenem Servomotor. Im Menü müssen Sie einen Test auswählen und die Position der Drossel auf der Welle so anpassen, dass die Drossel in geschlossener Position parallel zur langen Seite des Servomotors liegt.

![Setup servo iDreyer](../../img/air-damper/servo001.png)
![Setup servo iDreyer](../../img/air-damper/servo002.png)
![Setup servo iDreyer](../../img/air-damper/servo003.png)
![Setup servo iDreyer](../../img/air-damper/servo004.png)

## Montage

Installieren Sie die Montage der Drossel und des Servomotors im Basisteil.
Befestigen Sie es mit dem Befestigungsring. Es ist nicht erforderlich, den Servomotor und den Ring am Basisteil festzuschrauben, da das Gehäuse bei der endgültigen Montage mit Schrauben zusammengezogen wird und somit eine sichere Befestigung aller Komponenten gewährleistet wird.

Installieren Sie den Temperatur- und Feuchtigkeitssensor. Falls vorhanden, schneiden Sie ein passendes rechteckiges Stück Dämmmaterial zurecht und fügen Sie es wie auf dem Foto gezeigt ein.

![Setup servo iDreyer](../../img/air-damper/servo005.png)
![Setup servo iDreyer](../../img/air-damper/servo006.png)
![Setup servo iDreyer](../../img/air-damper/servo007.png)
![Setup servo iDreyer](../../img/air-damper/servo008.png)
![Setup servo iDreyer](../../img/air-damper/servo009.png)
![Setup servo iDreyer](../../img/air-damper/servo010.png)

## Überprüfung

Nach der Montage der Hauptbaugruppe sollten Sie das Verhalten des Geräts beim Einschalten des Motors beachten: Wenn die Drossel verklemt, kann es zu einem erheblichen Spannungsabfall kommen, der zu einem Neustart des Microcontrollers führt. Wenn das Gerät während des Betriebs unerwartet neu gestartet wird, überprüfen Sie die Drossel auf mechanische Blockierungen.

Es wird empfohlen, die Funktion der Drosselbaugruppe vor ihrer endgültigen Installation im Gehäuse zu überprüfen. Hierzu kann eine vorherige Montage der Steuerplatine und das Flashen des Microcontrollers erforderlich sein. Darüber hinaus ist die Verwendung eines separaten Geräts zum Testen von Servomotoren zulässig. Falls die Platine nicht vorbereitet ist, kann die Baugruppe mit anschließender Überprüfung nach der Elektronik-Montage installiert werden.
