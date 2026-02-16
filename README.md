# ZIN-70 Quad Nixie Display
 
### Important Notes

This is a four tube display built using Millclock ZIN-70 Nixie Tubes. This can be used to drive a clock, or just as a numeric display.

Please note that if you decide to use this diaply as a clock, it does not include colons.

### Components and Requirements

Supply:
* Any* 12V 500mA (or better) supply. DC 5.5mm Male Plug

Mechanical and Connectors:
* 1x PJ-063AH DC 5.5mm Female Connector 
* 1x DP62J12S202HQ DPDT Slide Switch (Power Switch)
* 2x TS04-66-85-BK-100-SMT SPST Button (Hour and Minute buttons)

Tubes:
* 4x ZIN-70 Nixie Tubes (Z5680M Pinout) - 170V ~5mA each

Passives:
* 4x 6kR 1206(in) SMD Current-Limiting Power Resistors
* 8x 1kR 1206(in) SMD Current-Limiting Signal Resistors
* 2x 100nF 1206(in) SMD Decoupling Capacitors

HV Boost Supply:
* 1x Omnixie NCH8200HV (12V to 170V 30mA)
    - Custom footprint. Only compatible with NCH8200V.

Driver:
* 1x DRM1-S 12-5V DC-DC Converter 
    - Custom footprint for this device. Swap or remove as required
* 1x ESP32 devboard 
    - Custom footprint for ESP32 WROOM 32D - SWAP FOR YOUR DRIVER. They are unlikely to match

Registers:
* 1x CD40109BPWRE4 TSSOP-16 4bit 3V to 18V Level Converter
    - Configured for 3.3V to 12V conversion specifically for ESP32. Adjust Vcc and Vdd as required.
* 2x HV5122 PQFP-44 32bit HV Registers (220V 100mA Drains)
