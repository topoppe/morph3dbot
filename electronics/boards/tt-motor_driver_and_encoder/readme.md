# TT-Motor-Platine

Die TT-Motor-Platine stellt einen Sonderfall dar: Sie besitzt eine andere Form als die restlichen *Morph3DBot*-Platinen.
Sie ist dazu gedacht, direkt auf TT-Motoren montiert zu werden.

Es ist ein Motortreiber IC A4953 verbaut, der einen Motor mit Systemspannung und einer Stromstärke von bis zu 2 Ampere versorgen kann.
Angesteuert wird der Treiber durch einen ATTiny44.

Weiter sind 4 Anschlüsse für Drehencoder des Motors vorhanden. Auch diese Anschlüsse sind mit dem ATTiny verbunden.

Die Platine bestitzt den selben Steckkontakt wie die restlichen *Morph3DBot*-Platinen, sodass ein Motor mit einer solchen Platine direkt in das System gehangen werden können.

Über eine DIP-Schalter-Reihe lässt sich die I2C-Adresse der Platine einstellen, so dass bis zu 8 Motoren im System verbaut werden können.
