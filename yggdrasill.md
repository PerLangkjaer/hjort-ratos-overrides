# Yggdrasill wiring guide

This guide describes how the cables are connected to the Octopus Max EZ board for the Rapunzel machine (code name Yggdrasill). Use it as a reference for wiring.

## Motors

- **X motor (T0)** – Motor1
- **X1 motor** – Motor2
- **Y motor** – Motor10
- **Y1 motor** – Motor9
- **Z motor (left)** – Motor5
- **Z1 motor (rear)** – Motor6
- **Z2 motor (right)** – Motor7
- **Extruder T0** – Motor3

## Heaters and sensors

- **Chamber heater**: port E1 (heater pin PA0).
- **Chamber heater thermistor**: TH1.
- **Chamber temperature sensor**: TH3.
- **Extruder body temperature sensor**: TH2.
- **Bed heater**: E2.

## Fans and lighting

- **Part‑cooling fan**: FAN4 (4‑pin digital PWM).
- **Hotend fan**: FAN1.
- **Controller fan**: FAN2.
- **Chamber heater circulation fan**: FAN3.
- **Filter or circulation fan in the chamber**: FAN6.
- **LED lighting**: FAN0.

## Sensors and buttons

- Filament runout: M6‑DET (PC15).
- Filament clog sensor: M5‑DET (PF1).
- Trigger Feeding button: M4‑DET (PF3).
- Trigger Retraction button: M3‑STOP (PF4).
- Y endstop: Y‑STOP.
- Probe/Beacon: PROBE or SERVO port.

## Miscellaneous

- RGB lighting: ports RGB1 (PE10) or RGB2 (PE9).
- PS‑ON / PWRDET for power supply: PF13 / PF12.
