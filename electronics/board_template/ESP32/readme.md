# ESP32 Board Template

Bei der ESP32 Platine handelt es sich um eine Arduino-IDE-Kompatible Basisplatine.
Diese Platine kann sowohl als Hauptplatine im System, als auch als Slave-Platine genutzt werden.

## Spannungsversorgung
Auf der Platine sind zwei Linearregler verbaut. Sie erzeugen aus der Versorgungsspannung des Systems stabile 5V und 3,3V Spannungsversorgungen für den Controller sowie weitere Peripherie.

## Controller
Herzstück der Platine ist ein ESP32-Wroom Modul von Espressif. Es ist der selbe Controller-Typ, der auch auf Node-MCU Boards verbaut ist.
Neben den Interfaces der AT-Mega-Platine bietet das Modul auch WLAN und Bluetooth Konnektivität.

## USB-Interface
Ein CP2104 Chip verbindet die UART-Schnittstelle des Controllers mit einer USB-Buchse. Hierüber ist eine Kommunikation mit einem PC und die Programmierung mittels der Arduino-IDE möglich.

## Erweiterungsschnittstelle
Auf der Oberseite der Platine sind zwei doppelreihige Buchsenleisten mit jeweils 12-Anschlüssen vorhanden. Hier können +5V, +3,3V, Ground, UART sowie die meisten Pins des Controllers abgegriffen werden.
So ist es möglich, eigene Erweiterungen anzuschließen.
