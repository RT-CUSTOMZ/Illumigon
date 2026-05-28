# 💡 Illumigon

Die modularen smarten Leuchtpanels mit Wifi-Konnektivität, die Ihr auf der Campuswoche bauen könnt.

---

## 📦 Features

- [x] Individuell adressierbare LEDs (WS2811)
- [x] WLAN-fähige Steuerung via ESP32
- [x] Konfigurierbare Animationen und Farbpaletten
- [x] Open Source Hardware + Software (WLED)
- [x] Home Assistant Integration
- [x] Modular steckbar
- [x] Keine Kabelsalat

---

## 📁 Dateiübersicht

| Pfad / Datei                | Beschreibung                           |
|----------------------------|-----------------------------------------|
| `Fusion 360/`              | Fusion 360 Archiv und STEP-Modell       |
| `Gerber/`                  | Leiterplattenlayouts im Gerber Format   |
| `KiCad/`                   | Leiterplattenlayouts im KiCad 9 Format  |
| `STLs/`                    | 3D-Modell im STL-Format für den 3D-Druck|
| `SVGs/`                    | Vectorgrafiken zum Laserschneiden und Gravieren      |

## 🧾 Stückliste / Teilebestellung

### 🧠 ESP32 WLED Controller

| Bauteil                 | Referenz                    | Wert                        | Footprint             | Menge | Link  |
|-------------------------|-----------------------------|-----------------------------|-----------------------|-------|-------|
| Keramikkondensator      | C3, C4, C5, C7, C8, C9, C10 | 100n                        | SMD 1206              | 7     |       |
| Keramikkondensator      | C11, C12                    | 22u                         | SMD 1206              | 2     |       |
| Elektrolytkondensator   | C1                          | 470u                        | C_Elec_10x10.2        | 1     |       |
| Keramikkondensator      | C2                          | 1u0                         | SMD 1206              | 1     |       |
| Keramikkondensator      | C6                          | 10u                         | SMD 1206              | 1     |       |
| Dichschichtwiderstand   | R3, R6, R9                  | 100R                        | SMD 0805              | 3     |       |
| Dichschichtwiderstand   | R8, R11, R12                | 10K                         | SMD 1206              | 3     |       |
| Dichschichtwiderstand   | R4, R5                      | 5K1                         | SMD 1206              | 2     |       |
| Dichschichtwiderstand   | R7, R10                     | 4K7                         | SMD 0805              | 2     |       |
| Dichschichtwiderstand   | R1                          | 2K0                         | SMD 0805              | 1     |       |
| Dichschichtwiderstand   | R2                          | 470R                        | SMD 0805              | 1     |       |
| Leistungsinduktor       | L1                          | 4u7                         | 7.3x6.6mm             | 1     |       |
| Leuchtdiode             | D1, D2, D3, D5, D6          | LED                         | SMD 0805              | 5     |       |
| Schottky-Diode          | D4, D7                      | SS34                        | SMA                   | 2     |       |
| 3.3V Spannungswandler   | U1                          | AMS1117-3.3                 | SOT-223-3             | 1     |       |
| 32-bit Mikrocontroller  | U2                          | ESP32-WROOM-32E             |                       | 1     |       |
| 5V Synchr.-Schaltregler | U3                          | AP63205WU                   | TSOT-23-6             | 1     |       |
| 420Mbps Levelshifter    | U4                          | SN74LVC1T45DBV              | SOT-23-6              | 1     |       |
| USB-UART Transceiver    | U5                          | CH340C                      | SOIC-16               | 1     |       |
| Bipolartransistor       | Q2, Q3                      | BC857                       | SOT-23                | 2     |       |
| Bipolartransistor       | Q4, Q5                      | MMBT3904                    | SOT-23                | 2     |       |
| P-Kanal MOSFET          | Q1                          | Q_PMOS_GDS                  | TO-252-2              | 1     |       |
| USB-C-Buchse 16-Pin     | J1                          | USB_C_Receptacle_USB2.0_16P | GCT USB4105           | 1     |       |
| Hohlsteckerbuchse       | J2                          | Barrel_Jack_Switch          |                       | 1     |       |
| Pinheader 2.54 2x3      | J3                          | Conn_02x03_Odd_Even         | 2x03 P2.54mm Vertical | 1     |       |

### 💡 Komponenten je Panel

| Bauteil        | Referenz    | Wert       | Footprint                | Menge | Link |
|----------------|-------------|------------|--------------------------|--------|------|
| Platine        | Ecke        |            |                          | 3      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/Gerber/Ecke.zip) |
| Platine        | Seite       |            |                          | 3      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/Gerber/Seite.zip) |
| Plexiglas      | Lichtleiter | 4mm klar   | Acrylglas GS             | 1      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/e6f71768b751d2ca16ff6e7ad1a84dd5374f7dc3/SVGs/Light_Guide_Panel_fein.svg) |
| Plexiglas      | Diffusor    | 3mm opal   | Acrylglas XT opal 70105  | 1      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/e6f71768b751d2ca16ff6e7ad1a84dd5374f7dc3/SVGs/Diffusor.svg) |
| Pinheader 2x3  | J1          | 02x03      | Vertikal                 | 3      | [LCSC](https://www.lcsc.com/product-detail/C492420.html) |
| Pinheader 1x5  | J2, J3      | 01x05      | Horizontal               | 6      | [LCSC](https://www.lcsc.com/product-detail/C492413.html) |
| Platine        | Verbinder   |            |                          | 1      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/Gerber/Verbinder.zip) |
| Pinsocket 2x3  | J1, J2      | 02x03      | Vertikal                 | 2      | [LCSC](https://www.lcsc.com/product-detail/C5116527.html) |
| Pinheader 1x2  | J3, J4      | 01x02      | Vertikal                 | 2      | [LCSC](https://www.lcsc.com/product-detail/C492401.html) |
| Jumper 1x2     |             | 01x02      |                          | 1      | [LCSC](https://www.lcsc.com/product-detail/C100114.html) |
| Schraube       |             | PZ 3x10    |                          | 3      | [Schraubenhimmel](https://www.schraubenhimmel.de/schrauben/senkkopf/spanplattenschrauben-kreuzschlitz/65940/spax-wirox-senkkopf-kreuzschlitz-pz-1-3x10-mm-vollgewinde) |
| 3D-Druck       |             | Deckel u.  |                          | 3      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/STLs/Deckel_unten%20v49.stl) |
| 3D-Druck       |             | Deckel m.  |                          | 3      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/STLs/Deckel_mitte%20v45.stl) |
| 3D-Druck       |             | Verbinder  |                          | 2      | [GitHub](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/STLs/Verbinder%20v9.stl) |



