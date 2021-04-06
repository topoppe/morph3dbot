# *Morph3DBot*-Platinen

Alle Platinen für das *Morph3DBot* System haben den selben Formfaktor und werden auf die Basisstruktur montiert.
Die Platinen werden untereinander mit einem vierpoligen Kabel verbunden. Über dieses Kabel werden die Platinen mit Strom versorgt und können
miteinander kommunizieren.

Die Kommunikation erfolgt über einen I2C-Bus, die Spannungsversorgung bringt die Batteriespannung an alle Platinen.

Jede Platine hat mindestens 2 Stecker zum verbinden mit anderen Platinen. Dadurch kann die Verkabelung zu den einzelnen Modulen
als Daisy-Chain ausgeführt werden und wird wesentlich vereinfacht.
Bei den meisten Platinen lässt sich die I2C-Adresse entweder per Software oder per DIP-Schalter einstellen.

Bis jetzt gibt es bereits folgende Platinen:
- Stromversorgung: Diese Platine darf und muss genau einmal im System verbaut werden. Hier wird die Stromquelle wie z.B. eine Batterie oder ein Netzteil angeschlossen. Außerdem sind hier die Pull-Up-Widerstände für den I2C-Bus verbaut.
- HUB-Platine: Dient als Verteiler. Hier können bis zu 8 weitere Platinen angeschlossen werden
- AT-Mega-328-Platine: Diese Platine ist mit einem ATMega328p Controller bestückt. Sie kann als "Gehirn" des Systems verwendet werden
- ESP32-Platine: Diese Platine ist mit einem ESP32-Wroom-Modul bestückt. Auch sie kann als "Gehirn" verwendet werden, besitzt aber auch WLAN und Bluetooth Schnittstellen
- Taster-Platine: Sie besitzt 5 Taster um eingaben ins System zu ermöglichen
- Ultrasonic-Platine: Hier kann ein 4-poliger Ultraschall Sensor angeschlossen werden
- Motor-und-Servo-Platine: An dieser Platine können 8 Servos sowie 2 Gleichstrommotoren angeschlossen werden
- Servo-Platine: Wie die Motor-und-Servo-Platine, jedoch ohne die Anschlüsse für die Gleichstrommotoren
- Line-Follower-Platine: Mit ihr kann eine Linie auf dem Boden erkannt werden
- Mikroe-Platine: Hier kann ein "Click-Board" von Mikroe.com angeschlossen werden

Zusätzlich gibt es eine Platine mit einem anderen Formfaktor: Die "TT-Motor-Platine". Diese Platine kann direkt auf die aus dem Maker-Bereich bekannten TT-Motoren geklebt werden. Sie besitzt eine I2C-Schnittstelle, einen Motortreiber sowie Eingänge für den Enkoder des Motors. Angeschlossen wird die Platine mit dem selben System wie die restlichen *Morph3DBot* Platinen.

Für die ATMega, die ESP32- sowie für die Platinen mit ATTINY-Controller stehen Templates im Repo bereit. Alle Grundbauteile sind bereits vorhanden, sodass eigene Platinen schnell erstellt werden können.
