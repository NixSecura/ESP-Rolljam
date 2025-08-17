
 🚀 ESP32 RollJam Project

 📖 Overview

This project is an > > ESP32-based RollJam device> >  designed for experimenting with > > RF security, wireless communication, and embedded systems> > .
It integrates:

>  > > ESP32-WROOM-32> >  microcontroller (WiFi + Bluetooth SoC)
>  > > CC1101 RF Transceiver> >  (for sub-GHz RF capture & replay)
>  > > SSD1306 OLED Display> >  (for live status/interaction)
>  > > Li-ion Battery Power Supply> >  with low-dropout regulator
>  > > User Controls> >  via tactile buttons

The main purpose of this project is > > educational & research use> > —to understand RF protocols, IoT security challenges, and embedded hardware design.

⚠️ > > Disclaimer:> >  This project is strictly for > > educational and research purposes only> > . Do not use it for unauthorized or illegal activities.



 🛠️ Features

>  📡 > > Sub-GHz RF Communication> >  with CC1101
>  🖥️ > > Real-time OLED Display> >  (0.96" SSD1306)
>  🔋 > > Battery Powered> >  with AP2112K-3.3 regulator
>  🎛️ > > User Input Buttons> >  for mode switching
>  💾 > > Open-source Hardware Files> >  (Schematics, PCB, Gerbers, BOM)



 🗂️ Repository Contents

>  > > /schematics/> >  → Circuit diagrams in PDF/PNG format
>  > > /pcb/> >  → PCB design files (EasyEDA/KiCad compatible)
>  > > /gerbers/> >  → Manufacturing-ready Gerber files
>  > > /bom/> >  → Bill of Materials (BOM) with components
>  > > /firmware/> >  → ESP32 source code & examples (Arduino/ESP-IDF) > (optional, if you upload)> 
>  > > README.md> >  → Documentation (this file)



 🔧 Hardware Details

 1️⃣ ESP32-WROOM-32

>  Dual-core microcontroller with WiFi + Bluetooth
>  Controls RF module & OLED
>  SPI interface for CC1101
>  I²C interface for SSD1306

 2️⃣ CC1101 RF Transceiver

>  Sub-GHz RF communication (315/433/868/915 MHz depending on module)
>  Interfaces with ESP32 via SPI (MISO, MOSI, SCK, CSN)
>  GDO0 & GDO2 used for interrupts/data handling

 3️⃣ SSD1306 OLED Display (I²C)

>  Resolution: 128×64
>  Connected via I²C (SCL = D22, SDA = D21)
>  Used to display RF logs, system info, and user feedback

 4️⃣ Power Supply

>  Li-ion Battery input (3.7–4.2V nominal)
>  AP2112K-3.3V LDO regulator for stable 3.3V output
>  On/Off power switch before regulator
>  Input/Output capacitors for stability (10µF)

 5️⃣ User Controls

>  Tactile switches connected to ESP32 GPIOs
>  Used for mode selection (e.g., scan, capture, replay)



 📋 Bill of Materials (BOM)

| Component                | Quantity | Notes                  |
|  | -- | - |
| ESP32-WROOM-32           | 1        | Main MCU               |
| CC1101 Module            | 1        | Sub-GHz RF transceiver |
| SSD1306 OLED 0.96"       | 1        | I²C version            |
| AP2112K-3.3 LDO          | 1        | 600mA LDO Regulator    |
| Li-ion Battery Connector | 1        | JST-PH 2.0             |
| Tactile Switches (SMD)   | 2        | For user input         |
| Capacitors 10µF          | 2        | Input/Output for LDO   |
| Resistors 10k            | 2        | Pull-ups for I²C       |



 ⚡ Getting Started

 🔹 Hardware Setup

1. Assemble PCB or wire components according to schematic.
2. Connect Li-ion battery (3.7–4.2V).
3. Ensure CC1101 is matched to correct RF band module.

 🔹 Software Setup

>  Install > > Arduino IDE> >  or > > ESP-IDF> > .
>  Install required libraries:

  >  `SPI.h` for CC1101 communication
  >  `Wire.h` + `Adafruit_SSD1306` for OLED
  >  `ELECHOUSE_CC1101_SRC_DRV.h` (popular CC1101 Arduino driver)
>  Upload firmware via USB-TTL or onboard programmer.



 📷 Project Images

(Add photos of PCB, assembled board, and working prototype here)



 ⚠️ Disclaimer

This project is created > > only for research, education, and security awareness> > .
⚡ Unauthorized use for signal hijacking, car key cloning, or any malicious activity is > > strictly prohibited> > .



 🏷️ Tags / Keywords

`ESP32` `CC1101` `RF Hacking` `IoT Security` `RollJam` `Wireless Security` `Embedded Systems` `PCB Design`

