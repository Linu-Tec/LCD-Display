# LCD-Display
Ein LCD Display per Arduino ansteuern

Aufgabe: Ein LCD Display soll mit einem Arduino Mikrocontroller angesteuert werden. Danach soll auf dem Display ein vorher festgelegter Text erscheinen.

Material: Arduino Mikrocontrollerboard (In diesem Beispiel UNO R3), ein Drehregler (bzw. Potentiometer), 14 Jumperkabel, Breadboard

Das vierzeilige LCD Modul mit angelötetem I²C Bus ermöglicht die Verwendung eines LCD Moduls mit einer einfachen Verkabelung. Dies ist bei komplexeren Projekten besonders vorteilhaft. Dieses I²C LCD Modul hat jeweils 20 Zeichen in 4 Zeilen zur Verfügung.

Um mit dem I²C LCD Modul zu arbeiten, benötigt man eine Library welche noch nicht im Arduino Programm vorinstalliert ist. Wir verwenden in dieser Anleitung die „LiquidCrystal I2C“ Library. Die Library kann über die Bibliothekenverwaltung der Arduino-Software hinzugefügt werden. Als Suchbegriff direkt den Namen „LiquidCrystal I2C“ eingeben.

Eine detaillierte Beschreibung, wie Bibliotheken eingefügt werden findet man im Theorieteil „Anleitungen für Arduino“ – „Hard und Software“ im Unterpunkt 2.2.2.“Bibliotheken zur Arduino Software hinzufügen“.
Material: Arduino / 4×20 Display mit I²C Modul / Kabel

Aufgabe: In jeder der 4 Zeilen einen Text anzeigen lassen.

Verkabelung: Die Verkabelung ist sehr simpel. Am I2C LCD Modul sind nur vier Kontakte vorhanden. GND wird natürlich mit dem GND Kontakt am Microcontroller verbunden. VCC mit dem 5V Kontakt am Microcontroller, SDA mit dem Analogen Eingang A4 und SCL mit dem Analogen Eingang A5.

Achtung!: Bei dem MEGA2560 R3 Microcontroller gibt es für die SDA – und SCL- Kontakte eigene Eingänge auf dem Board unter 20 und 21.

Auf der Rückseite des Displays, am I2C Modul befindet sich ein blauer Kasten mit dem der Kontrast geregelt werden kann, so ist kein zusätzlicher Drehregler im Aufbau nötig. Achtung: Oft ist der Kontrast zu Beginn sehr weit herunter geschraubt. Daher sollte man den Kontrast mit dem Drehregler erhöhen.
