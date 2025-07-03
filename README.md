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

| Bauteil                | Referenz                          | Wert              | Footprint                                                        | Menge    | Link |
|------------------------|-----------------------------------|-------------------|------------------------------------------------------------------|----------|-----------|
| Platine                |                                   | SMD Controller    |                                                                  | 1        | [Github](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/Gerber/SMD_Controller.zip) |
| 3D-Druck               |                                   | Controller Gehäuse Unterseite        |                                                                  | 1        | [Github](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/STLs/SMD_Controller_Geh%C3%A4use_Unterseite_v10.stl) |
| 3D-Druck               |                                   | Controller Gehäuse Oberseite         |                                                                  | 1        | [Github](https://github.com/RT-CUSTOMZ/Illumigon/blob/V4/STLs/SMD_Controller_Geh%C3%A4use_Oberseite_v10.stl) |
| Keramikkondensator     | C5, C6, C7, C11, C12, C13, C14    | 100nF             | SMD 1206 | 7        | [LCSC](https://www.lcsc.com/product-detail/C24497.html) |
| Keramikkondensator     | C3, C4                            | 22uF              | SMD 1206                      | 2        | [LCSC](https://www.lcsc.com/product-detail/C77091.html) |
| Keramikkondensator     | C1                                | 10uF              | SMD 1206                      | 1        | [LCSC](https://www.lcsc.com/product-detail/C13585.html) |
| Elektrolytkondensator  | C9                                | 470uF             | SMD 10,2x10,2x10,5                                                   | 1        | [LCSC](https://www.lcsc.com/product-detail/C72519.html) |
| Keramikkondensator     | C10                               | 1uF               | SMD 1206                      | 1        | [LCSC](https://www.lcsc.com/product-detail/C1848.html) |
| Dickschichtwiderstand  | R3, R4, R5                        | 10kOhm            | SMD 1206                      | 3        | [LCSC](https://www.lcsc.com/product-detail/C17902.html) |
| Dickschichtwiderstand  | R6, R8                            | 5,1kOhm           | SMD 1206                      | 2        | [LCSC](https://www.lcsc.com/product-detail/C2907509.html) |
| Dickschichtwiderstand  | R7                                | 30Ohm             | SMD 1206                      | 1        | [LCSC](https://www.lcsc.com/product-detail/C25373.html) |
| Leistungsinduktor      | L1                                | 4.7uH             | SMD 7,1 x 6,6                                          | 1        | [LCSC](https://www.lcsc.com/product-detail/C41410634.html) |
| Schottky-Diode         | D2, D3                            | SS34              | SMD SMA                                              | 2        | [LCSC](https://www.lcsc.com/product-detail/C8678.html) |
| USB-UART Transceiver   | U1                                | CH340C            | SOIC-16                                       | 1        | [LCSC](https://www.lcsc.com/product-detail/C84681.html) |
| 32-bit Mikrocontroller | U2                                | ESP32-WROOM-32E   |                                                   | 1        | [LCSC](https://www.lcsc.com/product-detail/C701342.html) |
| 5V Synchr.-Schaltregler| U3                                | AP63205WU         | TSOT-23-6                                                        | 1        | [LCSC](https://www.lcsc.com/product-detail/C2071056.html) |
| 420Mbps Levelshifter   | U4                                | SN74LVC1T45DBV    | SOT-23-6                                           | 1        | [LCSC](https://www.lcsc.com/product-detail/C7843.html) |
| 3.3V Spannungswandler  | U6                                | AMS1117-3.3       | SOT-223-3                                                | 1        | [LCSC](https://www.lcsc.com/product-detail/C347222.html) |
| NPN Bipolar Transistor | Q1, Q2                            | MMBT3904          | SOT-23                                             | 2        | [LCSC](https://www.lcsc.com/product-detail/C20526.html) |
| P-Kanal Mosfet         | Q4                                | AOD403 oder 40P04 | TO-252-2 GDS                                                     | 1        | [LCSC](https://www.lcsc.com/product-detail/C5224305.html) |
| Klinkenbuchse          | J1                                | 2,5x6,3mm         |                                             | 1        | [LCSC](https://www.lcsc.com/product-detail/C720558.html) |
| USB-C-Buchse           | J2                                | USB2.0 16P        | USB-C 16P         | 1        | [LCSC](https://www.lcsc.com/product-detail/C2765186.html) |
| Pinheader 2x3          | J3                                | 02x03             | 2x03 P2.54mm                                  | 1        | [LCSC](https://www.lcsc.com/product-detail/C492420.html) |
| Steckernetzteil        |                                   | 12V/2,5+A         |                                                                  | 1        | [Reichelt](https://www.reichelt.de/de/de/shop/produkt/steckernetzteil_36_w_12_v_3_a-171106) |
| Hohlstecker            |                                   | 2,5x5,6mm         |                                                                  | 1        | [Reichelt](https://www.reichelt.de/de/de/shop/produkt/hohlstecker_knickschutz_aussen_5_5_mm_innen_2_5_mm-8648) |

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



