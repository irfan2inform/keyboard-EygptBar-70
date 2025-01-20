Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
# EygptBar-70
A 5*14keys ortholinear HID keyboard using ATmega328P as MCU. Hotswap sockets for MX, One LED indicator(default as Caps_lock))

![P_20250119_000836](https://github.com/user-attachments/assets/5616d02a-8f3d-4b46-9daa-9eff89a8c298)

#BOM
| Quantity | Comment       | Designator          | Footprint                         |
| -------- | ------------- | ------------------- | --------------------------------- |
| 4        | 22pF          | C1,C2,C6,C9         | CAP-TH_L4.8-W3.2-P5.08-D0.5       |
| 3        | 100nF         | C3,C4,C8            | C1206                             |
| 4        | 47uF          | C6,C6,C6,C6         | CAP-SMD_L3.5-W2.8-R-RD            |
| 1        | 10uF          | C7                  | C0603                             |
| 1        | 1uF           | C10                 | C0603                             |
| 1        | 2.54-2P       | CN1                 | CONN-TH_2P-P2.54_C9900022459      |
| 5        | XH-4AW        | CN2,CN3,CN4,CN5,CN6 | CONN-TH_XH-4AW                    |
| 2        | TC1N4729ATB   | D1,D2               | DO-41_BD2.4-L4.7-P8.70-D0.9-FD    |
| 1        | SMF5.0CA      | D3                  | SOD-123_L2.7-W1.8-LS3.7-BI        |
| 2        | 1.5kΩ         | R1,R3               | RES-TH_BD1.9-L3.3-P7.30-D0.5      |
| 1        | 10kΩ          | R2                  | RES-TH_BD1.8-L3.2-P7.20-D0.4      |
| 1        | 3.4kΩ         | R4                  | R0603                             |
| 1        | TS-1086S-B3   | SW1                 | KEY-SMD_4P-L6.0-W4.0-P3.40-LS5.6  |
| 1        | CapLockLED    | U1                  | LED-TH_BD3.0-P2.54-FD             |
| 2        | 75Ω           | U2,U3               | RES-TH_BD2.3-L3.7-P7.70-D0.9      |
| 1        | ATMEGA328P-PU | U4                  | DIP-28_L34.6-W7.3-P2.54-LS10.2-BL |
| 1        | AVRISP_-6     | U5                  | AVRISP                            |
| 1        | ER20BGFBK     | U6                  | CONN-TH_ER20BGFBK                 |
| 1        | CH334R        | U8                  | QSOP-16_L4.9-W3.9-P0.635-LS6.0-BL |
| 1        | SY6280AAC     | U9                  | SOT-23-5_L3.0-W1.7-P0.95-LS2.8-BR |
| 1        | 16MHz         | X1                  | HC-49US_L11.5-W4.5-P4.88          |
| 1        | 12MHz         | X2                  | HC-49S_L11.5-W5.0-P4.88           |
