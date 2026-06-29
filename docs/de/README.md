# iDryer X

!!! note "Wie man diesen Abschnitt liest"

    Die X-Serie hat sich im Laufe der Zeit entwickelt. Die Versionen sind nummeriert – eine höhere Nummer bedeutet eine neuere und aktuellere Version.

Die X-Serie wurde auf eine neue Plattform migriert. Weitere Informationen finden Sie im Abschnitt iDryerControllerV2.

## iDryerControllerV2

Die neue Version basiert auf einem leistungsstärkeren Controller und wird als fertige Leiterplatte vom Hersteller geliefert. Eine manuelle Montage ist nicht erforderlich. Der Controller bietet spezialisierte Anschlüsse, die die Integration zusätzlicher Peripherie vereinfachen.

## iDryerController

Die Unterstützung der iDryerController-Plattform wird hauptsächlich von Mitgliedern der Community fortgesetzt.

Eine universelle Filament-Trockenlösung für 3D-Druck-Enthusiasten.
Sie können sie aus verfügbaren und günstigen Komponenten zusammenbauen – beispielsweise aus einem alten Heizer eines Hotends, einem unnötigen Lüfter und einem Kühlkörper. Als Gehäuse kann eine Kiste vom Baumarkt und eine beliebige Isolierung verwendet werden. Die Liste der verwendeten Teile ist nur durch Ihre Fantasie begrenzt.

Lösungen für Enthusiasten finden Sie im Bereich DIY.

Ein KIT-Set ist ebenfalls erhältlich, das alles Notwendige enthält, einschließlich vorbearbeiteter Gehäuseteile, Elektronik, Metalleile für den Boden und Spulenhalterfeste, Heizer und Lüfter.
Anweisungen zur Montage des KIT-Sets finden Sie im Abschnitt iDryer v3.

## Vorteile des Trockners

## Funktionen

### Trocknung
- Auswahl der Temperatur und Trocknungszeit
- genaue Aufrechterhaltung der gewählten Temperatur
- Anzeige der aktuellen Feuchte
- automatische Umschaltung in den Lagermodus

### Lagerung
- Aufrechterhaltung der eingestellten Feuchte
- automatisches Ein-/Ausschalten des Heizers und der Konvektion beim Erreichen der festgelegten Feuchte
- Lagerdauer ist zeitlich unbegrenzt

### Voreinstellungen
- Auswahl einer Voreinstellung für häufig verwendete Kunststoffe
- Einstellung der Temperatur und Zeit für jede Voreinstellung

### Wägen
- Wiegen von Filament
- Einstellung des Behältergewichts
- Einstellung des Schwellwertes für die Filamentendsignalisierung
- Signalisierung zum Filamenende (Ton oder Triggerausgang)

### Kammerlüftung
- Klappe wird von einem Servo angesteuert
- Einstellung der Zeit "offen"
- Einstellung der Zeit "geschlossen"

### Allgemeine Funktionalität
- PID-Regelung der Heizleistung
- kunststoffsicherer Betrieb des Heizelementes
- genaue Aufrechterhaltung der gewählten Temperatur
- Feuchteüberwachung in der Kammer

### Energieeffizienz
- Trockenmodus ~ 40W/Stunde
- Lagermodus ~ 20W/Stunde
- Standby-Modus ~ 3W/Stunde

---

## Firmware
[Firmware-Datei](https://github.com/pavluchenkor/iDryerController/blob/master/src/Configuration.h) enthält alle möglichen Optionen und Firmware-Konfiguration

### Firmware für Arduino-Bootloader

!!! warning "Nicht empfohlen"

  - kein WDT
  - keine Servo-Unterstützung
  - keine zusätzliche PWM-Kanalunterstützung
  - es wird keine Waage für Spulen im Trockner geben
  - weitere Entwicklung findet nicht statt

### Firmware für Minicore-Kern

  - funktionierender Watchdog-Timer / startet die Firmware bei Fehler neu
  - Servo-Antriebsunterstützung
  - Unterstützung des zusätzlichen PWM-Kanals
  - erweitertes Menü und Funktionen
  - Firmware-Sicherheit

> Die Firmware für den Arduino-Kern kann in frühen Versionen verwendet werden, wird aber nicht empfohlen. Es ist besser, einen Programmierer zu kaufen, den Bootloader neu zu schreiben und die sichere Firmware zu verwenden.

!!! note annotate "Projektdateien auf GitHub"

    [iDryer v1 prototype](https://github.com/pavluchenkor/iDryer) - Prototyp des heutigen Trockners, eine sehr günstige und wirtschaftliche Methode zum Kunststofftrocknen
    <!-- TODO: добавить ссылку на проект сушильного шкафа на esp32 по готовности проекта -->
    [iDryer v3](https://github.com/pavluchenkor/iDryerController) - aktuelle Version des Trockners mit Open-Source-Code. Das Repository enthält die Firmware und die Original-Projektdateien
