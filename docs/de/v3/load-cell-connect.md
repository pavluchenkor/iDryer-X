# Wägezellverbindung

Für den korrekten Betrieb des Wägungssystems in iDryer ist es erforderlich, die Kabel von der Wägezelle ordnungsgemäß mit dem HX711-Modul zu verbinden. Folgen Sie der nachstehenden Anleitung.

## Verbindungsstruktur

Das System verwendet nur Wägezellen mit vier Drähten. Die Farbcodierung ist normalerweise wie folgt:

- **Rot**: Stromversorgung + (Excitation+, E+)
- **Schwarz**: Stromversorgung - (Excitation-, E-)
- **Grün**: Signalausgabe + (Signal+, A+)
- **Weiß**: Signalausgabe - (Signal-, A-)

## Schaltplan für die Verbindung mit dem HX711-Modul

| Kabel von der Wägezelle | Anschluss am HX711-Modul |
|:----------------------|:------------------------|
| Rot (E+)           | E+                       |
| Schwarz (E-)            | E-                       |
| Grün (A+)           | A+                       |
| Weiß (A-)             | A-                       |

## Verfahren zur Überprüfung von Drähten mit einem Multimeter

Wenn Sie sich bei den Drahtfarben nicht sicher sind, können Sie die Bestimmung mit einem Multimeter durchführen:

**Stellen Sie das Multimeter in den Widerstandsmessmodus (Ohm) ein**.

**Finden Sie Drahtpaare mit ähnlichem Widerstand**:

- Messen Sie den Widerstand zwischen allen möglichen Drahtpaaren.
- Finden Sie zwei Drahtpaare, zwischen denen der Widerstand etwa 350-450 Ohm beträgt (für die meisten Standard-Wägezellen).

**Stromkreisbestimmung**:

- Ein Paar ist die Stromversorgung (Excitation+, Excitation-).
- Das andere Paar sind die Signalausgänge (Signal+, Signal-).
- In der Regel sind Schwarz und Rot die Masse bzw. Stromversorgung

**Wie man bestimmt, welcher Draht A+ und welcher A- ist**:

- Verbinden Sie das Multimeter im Modus zur Messung von Gleichspannung in Millivolt (mV DC).
- Verbinden Sie 5V Stromversorgung mit dem Stromversorgungsdrahtpaar (z.B. von einem DC-DC-Wandler der Controllerplatine).
- Verbinden Sie die Multimeter-Messspitzen mit dem Signaldrahtpaar.
- Wenn die Spannung positiv ist, ist das Kabel, das mit der roten Sonde verbunden ist, A+. Wenn die Spannung negativ ist, tauschen Sie die Sonden aus.
Zusätzlich:
- Drücken Sie auf die Wägezelle.
- Wenn sich die Spannung am Multimeter beim Drücken der Wägezelle erhöht, ist der Draht, der mit der roten Sonde des Multimeters verbunden ist, A+.
- Wenn die Spannung abnimmt (ins Negative geht), tauschen Sie die Sonden aus.

## Verbindungsschritte

- **Bestimmen Sie die Bestimmung jedes Drahtes** mit der oben beschriebenen Methode.
- **Vorbereitung der Kabel**: Isolierung an den Enden um 3-5 mm abisolieren.
- **Löten Sie die Kabel an die HX711-Platine** gemäß der Verbindungstabelle.
- **Beachten Sie die richtige Nummerierung der Wägezellen nach der Markierung auf der Platine**
- **Überprüfen Sie die Lötqualität**: Stellen Sie sicher, dass es keine Kurzschlüsse zwischen benachbarten Kontakten gibt.

## Wichtige Hinweise

- Das Gerät verwendet nur vierdrähtige Wägezellen.
- Falsche Verbindung kann zu fehlerhaftem Betrieb der Waage oder Beschädigung der Module führen.
- Nach dem Anschließen muss die Waage durch das Geräte-Menü kalibriert werden. Gehen Sie dazu in den Kalibrierungsmodus der Waage und folgen Sie den Anweisungen auf dem Bildschirm.
- Wenn EEPROM überschrieben wird, wird die Waagenkalibrierung erneut durchgeführt.
