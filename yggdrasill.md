# Rapunzel wiring guide

Detta schema visar hur kablarna kopplas till Octopus Max EZ for Rapunzel-maskinen. Anvand det som referens for att se hur allt ar anslutet.

## Motorer

- **X-motor (T0)** – Motor1
- **X1-motor** – Motor2
- **Y-motor** – Motor10
- **Y1-motor** – Motor9
- **Z-motor (vanster)** – Motor5
- **Z1-motor (bak)** – Motor6
- **Z2-motor (hogre)** – Motor7
- **Extruder T0** – Motor3

## Varmare och sensorer

- **Kammarvarmare**: port E1 (heater_pin PA0).
- **Kammarvarmarens termistor**: TH1.
- **Kammartemperaturgivare**: TH3.
- **Extruderhusets temperaturgivare**: TH2.
- **Baddvarmare**: E2.

## Flaktar och belysning

- **Part-cooling-flakt**: FAN4 (4-pin digital PWM).
- **Hotend-flakt**: FAN1.
- **Controller-flakt**: FAN2.
- **Kammarvarmarens cirkulationsflakt**: FAN3.
- **Filter- eller cirkulationsflakt i kammaren**: FAN6.
- **LED-belysning**: FAN0.

## Sensorer och knappar

- Filament runout: M6-DET (PC15).
- Filament clog-sensor: M5-DET (PF1).
- Trigger Feeding-knapp: M4-DET (PF3).
- Trigger Retraction-knapp: M3-STOP (PF4).
- Y-endstop: Y-STOP.
- Probe/Beacon: PROBE eller SERVO-porten.

## Ovrigt

- RGB-belysning: portarna RGB1 (PE10) eller RGB2 (PE9).
- PS-ON / PWRDET for nataggregat: PF13 / PF12.
