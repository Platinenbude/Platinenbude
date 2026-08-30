# 🕰️ RGB-LED-Matrix-Uhr (Arduino)

![<img width="1408" height="768" alt="image" src="https://github.com/user-attachments/assets/01b59fa3-4eda-4d60-b2a9-2f0af0bc5604" />
)

Willkommen im offiziellen GitHub-Repository der **Platinenbude**! 
Hier findest du alle wichtigen Unterlagen, Schaltpläne und Daten für den Nachbau der RGB-LED-Matrix-Uhr.

## 📺 Zum YouTube-Video
Die komplette Schaltplan-Analyse und die technische Erklärung zu diesem Projekt findest du auf meinem Kanal.
👉 **[Hier geht's zum Video auf YouTube](Video Link folgt)**

## 🛠️ Stückliste (Kern-Komponenten)
Für den Aufbau der Steuerung (siehe Schaltplan) werden unter anderem folgende Bauteile benötigt:
* **Microcontroller:** Arduino 
* **Echtzeituhr (RTC):** DS3231 Modul (über I2C)
* **Schieberegister:** 74HC595N
* **Treiber-ICs:** ULN2003A
* **Transistoren:** BD140 (PNP) für das Anoden-Multiplexing
* **Spannungsregler:** 7805 (für stabile 5V)
* **Kondensatoren:** 100µF, 10µF (Elkos) und 100nF (Keramik) zum Abblocken
* **Widerstände:** Diverse (z.B. 10k Pull-Ups, 1k, 240 Ohm)
* **Stromversorgung:** 12V DC Netzteil

*(Pro-Tipp aus dem Video: Achtet beim Nachbau unbedingt auf die 10k Pull-Up-Widerstände an den Basen der BD140-Transistoren. Diese sind extrem wichtig, um "Ghosting" bei den Matrix-LEDs zu verhindern!)*

## 📂 Datei-Übersicht in diesem Ordner
* `Schaltplan_RTC_Clock.pdf` - Der detaillierte Schaltplan in der aktuellen, bereinigten Version.
* *(Weitere Dateien wie der Arduino-Code folgen)*

## ⚠️ Wichtiger Hinweis (Disclaimer)
Dies ist ein privates Hobby- und Maker-Projekt der Platinenbude. Der Nachbau erfolgt auf eigene Gefahr. Ich übernehme keine Haftung für eventuelle Schäden an Hardware, Bauteilen oder Personen. Bitte achtet beim Basteln immer auf die grundlegenden Sicherheitsregeln der Elektronik!
