# SW_BatteryDevice_blinky

Einfaches STM32-Ausgangsprojekt für die BatteryDevice-Hardware.

Das Projekt ist insbesondere für den Einsatz im Unterricht vorgesehen. Die
Hardwarekonfiguration des BatteryDevice ist bereits vollständig in der
STM32CubeMX-Konfigurationsdatei (`.ioc`) hinterlegt.

## Zweck des Projekts

Das Projekt dient als sicherer Ausgangspunkt für eigene Programme auf der
BatteryDevice-Platine.

Die für die Hardware relevanten Pins und Peripherieeinheiten sind bereits
passend konfiguriert. Dadurch können Programme entwickelt und auf die Platine
übertragen werden, ohne dass die grundlegende Hardwarekonfiguration jedes Mal
neu erstellt werden muss.

Insbesondere wird dadurch das Risiko reduziert, dass Ausgänge durch eine
fehlerhafte Pin-Konfiguration gegeneinander geschaltet werden und dadurch
Bauteile der Platine beschädigt werden.

> **Hinweis für Schüler:**  
> Die vorhandene Pinbelegung in der `.ioc`-Datei sollte nicht verändert werden,
> sofern dies nicht ausdrücklich Teil der Aufgabenstellung ist.

## Beispielprogramm

Das mitgelieferte Programm ist bewusst sehr einfach gehalten.

In der Hauptschleife wird die `Alive_LED` periodisch umgeschaltet: