# AT-Mega328 Board Template

Bei der AT-Mega Platine handelt es sich um eine Arduino-IDE-Kompatible Basisplatine.
Diese Platine kann sowohl als Hauptplatine im System, als auch als Slave-Platine genutzt werden.

## Spannungsversorgung
Auf der Platine ist ein Linearregler verbaut. Er erzeugt aus der Versorgungsspannung des Systems eine stabile 5V Spannungsversorgung für den Controller sowie weitere Peripherie.

## Programmierschnittstelle
Auf der Rückseite der Platine befindet sich eine ICSP-Schnittstelle mit Arduino-typischer Belegung

## Controller
Herzstück der Platine ist ein AT-Mega-328P Controller von Microchip. Es ist der selbe Controller-Typ, der auch auf Arduino Uno und Nano Boards verbaut ist.
Er ist mit einem externen 16MHz Quarz verbunden, um eine stabile Kommunikation zu ermöglichen.

## USB-Interface
Ein CP2104 Chip verbindet die UART-Schnittstelle des Controllers mit einer USB-Buchse. Hierüber ist eine Kommunikation mit einem PC und die Programmierung mittels der Arduino-IDE möglich.

## Erweiterungsschnittstelle
Auf der Oberseite der Platine sind zwei doppelreihige Buchsenleisten mit jeweils 12-Anschlüssen vorhanden. Hier können +5V, Ground, UART sowie die meisten Pins des Controllers abgegriffen werden.
So ist es möglich, eigene Erweiterungen anzuschließen.
