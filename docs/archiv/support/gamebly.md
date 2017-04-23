## Projektstatus

Befindet sich noch in der Entwicklung

Ein Tisch mit einer LED-Matrix in der Mitte, auf dem man spielen kann.

## Projektteilnehmer
Jasmin und David


## Verwendete Hardware
* NodeMCU-Board
* Apa102C-LED-Streifen
    * 3 x 5 Meter
    * 30 LEDs pro Meter

## Syntax highlighting demo

````arduino

int timer = 100;           // The higher the number, the slower the timing.

void setup() {
  // use a for loop to initialize each pin as an output:
  for (int thisPin = 2; thisPin < 8; thisPin++) {
    pinMode(thisPin, OUTPUT);
  }
}

void loop() {
  // loop from the lowest pin to the highest:
  for (int thisPin = 2; thisPin < 8; thisPin++) {
    // turn the pin on:
    digitalWrite(thisPin, HIGH);
    delay(timer);
    // turn the pin off:
    digitalWrite(thisPin, LOW);
  }

  // loop from the highest pin to the lowest:
  for (int thisPin = 7; thisPin >= 2; thisPin--) {
    // turn the pin on:
    digitalWrite(thisPin, HIGH);
    delay(timer);
    // turn the pin off:
    digitalWrite(thisPin, LOW);
  }
}

````

## Installation zur Benutzung des NodeMCU-Boards
Es müssen Treiber installiert werden (CP2102)
[Link](https://www.silabs.com/products/mcu/Pages/USBtoUARTBridgeVCPDrivers.aspx)

### Anschluss Apa102C-LED-Streifen
![Schaltplan](http://www.elec-tron.org/wp-content/uploads/2015/12/nodetoapaq102.png)

## Verwendete Tools
* [Plattformio](http://platformio.org) als Entwicklungsumgebung
* [Git-Hub](http://github.com) zur Versionierung des Codes

## Code
[Git-Repo](https://github.com/d-amend/Gamebly)

## Related Work

### All Pixel

https://github.com/ManiacalLabs/AllPixel

#### Pro

#### Kontra

- kein Mapping
