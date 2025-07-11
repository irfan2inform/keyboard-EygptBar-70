# EygptBar-70
is A 5×14 keys **ortholinear** HID keyboard with a USB hub feature, using the ATmega328P as the MCU. It includes one LED indicator (default set as Caps Lock). You can swap the MCU board or switch board with your favorite one.

![Image](https://github.com/user-attachments/assets/6a262bb4-1907-4117-9434-2a4f9b526387)

![Image](https://github.com/user-attachments/assets/c98a37a7-7a98-4a15-b124-bde146653b94)

![Image](https://github.com/user-attachments/assets/cb64b910-1d11-4d01-858b-4968a3f8ad01)


From Smoky. 
![P_20250119_000836](https://github.com/user-attachments/assets/5616d02a-8f3d-4b46-9daa-9eff89a8c298)

# PCB Design files using EasyEDA

<img width="1000" height="500" alt="Image" src="https://github.com/user-attachments/assets/7110c5b0-06f5-4c40-bfa1-682256565b5b" />
<img width="1919" height="1031" alt="Image" src="https://github.com/user-attachments/assets/d20f04b4-770a-41f1-882a-4e07124c459b" />
<img width="1919" height="1030" alt="Image" src="https://github.com/user-attachments/assets/9c5beb7b-e084-4e23-849e-a794d3162979" />
<img width="1919" height="1028" alt="Image" src="https://github.com/user-attachments/assets/fe4cb7c1-f438-4a30-b132-7d1cd72be601" />
<img width="1919" height="1032" alt="Image" src="https://github.com/user-attachments/assets/a3944268-a285-4e34-b91c-696efded876f" />
<img width="1919" height="1029" alt="Image" src="https://github.com/user-attachments/assets/e2215814-931b-4335-afb6-ea49e7ac3bdf" />
<img width="1919" height="1034" alt="Image" src="https://github.com/user-attachments/assets/071e9ebb-33e5-403d-a1dd-c59103b2f040" />
<img width="1917" height="1026" alt="Image" src="https://github.com/user-attachments/assets/767ff47c-61c6-4590-aeab-bdeb9794c287" />
<img width="1919" height="1028" alt="Image" src="https://github.com/user-attachments/assets/7dd48f32-8269-4986-998a-f3ca06c561db" />
<img width="1919" height="1031" alt="Image" src="https://github.com/user-attachments/assets/2f24d153-2fd9-4583-91db-7a02bd0362fd" />
<img width="1919" height="1026" alt="Image" src="https://github.com/user-attachments/assets/d4bbcf44-7fab-47ca-aa48-28f194faabc5" />
<img width="1919" height="1031" alt="Image" src="https://github.com/user-attachments/assets/680d831a-46a2-492a-a15b-e02680516967" />


# Firmware
[Complied](https://github.com/zzsmoky/EygptBar-70/blob/f129200ea4578f9158403ffde063f7f00f164ff5/qmk_firmware/zzsmoky_egyptbar.hex)
or
[You can complie your own](qmk_firmware/) with this [Doc](https://docs.qmk.fm/newbs_building_firmware)

Burn your ATmega328P with [Avrdude](https://github.com/avrdudes/avrdude) or [Avrdudess](https://github.com/ZakKemble/AVRDUDESS) with this line of command


```
-c [your_favorite_Programer_e.g. stk500v1] -p m328p -P [your_port_e.g. COM8] -e -U flash:w:"C:\[your_path]\zzsmoky_egyptbar.hex":a -U lfuse:w:0xD7:m -U hfuse:w:0xD0:m -U efuse:w:0xFC:m 

```

remember to:

Sets the low fuse byte to 0xD7.

Sets the high fuse byte to 0xD0.

Sets the extended fuse byte to 0xFC
 
 
 

PS: For those who want to compile their own firmware: it hasn’t been uploaded to the official QMK repo yet, but you can clone the [files](https://github.com/zzsmoky/EygptBar-70/tree/f129200ea4578f9158403ffde063f7f00f164ff5/qmk_firmware) to your local qmk_firmware_repository/keyboards/zzsmoky/egyptbar


# PCB
[EasyEDA Pro(嘉立创EDA专业版)](https://github.com/zzsmoky/EygptBar-70/blob/f129200ea4578f9158403ffde063f7f00f164ff5/PCB/EygptBar-70.epro)

# 3D files
[.STEP Files](https://github.com/zzsmoky/EygptBar-70/blob/f129200ea4578f9158403ffde063f7f00f164ff5/3D_Models.7z)

# BOM
| Quantity | Comment       | Designator          | Footprint                         |
| -------- | ------------- | ------------------- | --------------------------------- |
| 2        | 22pF          | C1,C2               | CAP-TH_L4.8-W3.2-P5.08-D0.5       |
| 2        | 20pF          | C6,C9               | CAP-TH_L4.8-W3.2-P5.08-D0.5       |
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


# Keymap
L0:
```
    /*
     * ┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┐
     * │ ` │ 1 │ 2 │ 3 │ 4 │ 5 │ 6 │ 7 │ 8 │ 9 │ 0 │ - │ = │Bsp│
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │Tab│ Q │ W │ E │ R │ T │ Y │ U │ I │ O │ P │ [ │ ] │ \ |
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │Cap│ A │ S │ D │ F │ G │ H │ J │ K │ L │ ; │ ' │Ent│Del|
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │Sft│ Z │ X │ C │ V │ B │ N │ M │ , │ . │ / │Sft│ ↑ │PSCR
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │Ctl│FN |GUI│Alt│   │   │   │Alt│FN │App│Ctl│ ← | ↓ │ → |
     * └───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┘
     */
```
(Switch to L1 when FN pressed)

L1:
```
    /*
     * ┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┐
     * │ESC│F1 │F2 │F3 │F4 │F5 │F6 │F7 │F8 │F9 │F10│F11│F12│INS│
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │                                           |🗣-|🗣+ |   |
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │                                                       |
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │                                               │PUP│   |
     * ├───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┼───┤
     * │                                           │HM │PDw|END│
     * └───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┘
     */
```
