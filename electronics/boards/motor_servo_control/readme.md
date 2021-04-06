# Motor- und Servoplatine
Die Motor- und Servoplatine besitzt keinen eigenen Controller. Statt ihrer ist ein I2C-Portexpander [PCA9685](https://www.nxp.com/docs/en/data-sheet/PCA9685.pdf) von NXP verbaut.
Die I2C-Adresse lässt sich über einen DIP-Schalter einstellen.

Die Servo-Anschlüsse sind mit den Ausgängen LED8 bis LED15 verbunden.
Über der Anschlussleiste der Servos kann man mit Hilfe eines Jumpers einstellen, ob die Servos mit Systemspannung oder mit 5V versorgt werden sollen.

Auf der Motor-Platine ist außerdem noch ein Motortreiber [TB6612FNG](https://toshiba.semicon-storage.com/info/docget.jsp?did=10660&prodName=TB6612FNG) von Toshiba verbaut.
An ihm können zwei Gleichstrommotoren angeschlossen werden. Die Verbindung zum Portexpander-Chip lautet:

- TB6612FNG PWM-A = PCA9685 PWM2
- TB6612FNG A-IN-1 = PCA9685 PWM4
- TB6612FNG A-IN-2 = PCA9685 PWM3
- TB6612FNG PWM-B = PCA9685 PWM7
- TB6612FNG B-IN-1 = PCA9685 PWM6
- TB6612FNG B-IN-2 = PCA9685 PWM5

Die DC-Motoren werden hierbei duch die Systemspannung versorgt.
