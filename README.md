# OpenBook, Boraciu Ionut-Sorin 335CA

# Description 

 OpenBook is an open-source, affordable e-book reader designed for mass production. The project focuses on accessibility, cost efficiency, and user control, providing a customizable reading experience with open hardware and software.

# Table of contents
1. [Description](#description)
2. [E-Book Reader Diagram](#e-book-reader-diagram)
3. [Bill of materials (BOM)](#bill-of-materials-bom)
4. [Hardware Functionality Description](#hardware-functionality-description)
5. [Estimated Power Consumption 🔋](#estimated-power-consumption-)
6. [Total estimated power consumtion ( assuming wifi active) 🔋](#total-estimated-power-consumtion--assuming-wifi-active-)
7. [Estimated battery life](#estimated-battery-life)
8. [ESP32-C6 Pin Usage](#esp32-c6-pin-usage)
9. [Pins explanation](#pins-explanation)

 # E-Book Reader Diagram

 ![Diagram Image](Images/diagram.png)

 # Bill of materials (BOM)
 | 🛠 Component | 🔗 Link | 📄 Datasheet |
 |-------------|--------|------------|
 | 112A-TAAR-R03_ATTEND |[Comet](https://store.comet.srl.ro/Catalogue/Product/43497/) | [Datasheet](https://store.comet.bg/download-file.php?id=27596) |
 | 744043680IND | [Mouser](https://eu.mouser.com/ProductDetail/Wurth-Elektronik/744043680?qs=PGXP4M47uW6VkZq%252BkzjrHA%3D%3D) | [Datasheet](https://www.we-online.com/components/products/datasheet/744043680.pdf) |
 | ADAFRUIT_LEDCHIP | [SnapMagic](https://www.snapeda.com/parts/KP-1608SURCK/Kingbright/view-part/?ref=search&t=LED%200603) | [Datasheet](https://www.snapeda.com/parts/KP-1608SURCK/Kingbright/datasheet/) |
 | BD5229G-TR | [Component Search Engine](https://componentsearchengine.com/part-view/BD5229G-TR/ROHM%20Semiconductor) | [Datasheet](https://datasheet.datasheetarchive.com/originals/distributors/Datasheets_SAMA/f2b9741ef86007909f138d561a359946.pdf) |
 | BUTTON_CUSYOMV1 | [Panasonic](https://industry.panasonic.com/global/en/products/control/switch/light-touch/number/evqpuj02k) | [Datasheet](https://industry.panasonic.com/global/en/downloads?tab=catalog&small_g_cd=203&part_no=EVQPUJ02K&q=RVZRUFVKMDJLJTdDMTMlN0MyMDMlN0MzNDU5JTdDMSU3QyU3QzIlN0NmYWxzZQ%3D%3D) |
 | CPH3225A | [SnapMagic](https://www.snapeda.com/parts/CPH3225A/Seiko+Instruments/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/CPH3225A/Seiko%20Instruments/datasheet/) |
 | DS3231SN | [SnapMagic](https://www.snapeda.com/parts/DS3231SN%23/Analog+Devices/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/DS3231SN%23/Analog%20Devices/datasheet/) |
 | EAGLE-LTSPICE_CC0402 | [Component Search Engine](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
 | ESP32-C6-WROOM-1-N8 | [SnapMagic](https://www.snapeda.com/parts/ESP32-C6-WROOM-1-N8/Espressif+Systems/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/ESP32-C6-WROOM-1-N8/Espressif%20Systems/datasheet/) |
 | ESP32_WROVER_AVX | [Mouser](https://eu.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D) | [Datasheet](https://eu.mouser.com/datasheet/2/40/schottky-3165252.pdf) |
 | ESP32_WROVER_BME680_BME680 | [SnapMagic](https://www.snapeda.com/parts/BME680/Bosch/view-part/?welcome=home) | [Datasheet](https://www.snapeda.com/parts/BME680/Bosch%20Sensortec/datasheet/) |
 | ESP32_WROVER_EAGLE-LTSPICE_C | [Component Search Engine](https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO) | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
 | ESP32_WROVER_EAGLE-LTSPICE_R | [Component Search Engine](https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO) | [Datasheet](https://www.yageo.com/upload/media/product/products/datasheet/rchip/PYu-RC_Group_51_RoHS_L_12.pdf) |
 | ESP32_WROVER_SPARKFUN-DISCRETESEMI | [Component Search Engine](https://componentsearchengine.com/part-view/DMG2305UX-7/Diodes%20Incorporated) | [Datasheet](https://www.diodes.com//assets/Datasheets/DMG2305UX.pdf) |
 | ESP32_WROVER_SPARKFUN-IC-POWER_SOT23-5 | [Mouser](https://eu.mouser.com/ProductDetail/Microchip-Technology/MCP73831T-2ACI-OT?qs=yUQqVecv4qvbBQBGbHx0Mw%3D%3D) | [Datasheet](https://eu.mouser.com/datasheet/2/268/MCP73831_Family_Data_Sheet_DS20001984H-3441711.pdf) |
 | ESP32C6_VARISTORCN1812 | [Mouser](https://ro.mouser.com/ProductDetail/EPCOS-TDK/B72520T0350K062?qs=dEfas%2FXlABIszF52uu7vrg%3D%3D) | [Datasheet](https://www.tdk-electronics.tdk.com/inf/75/db/CTVS_14/Surge_protection_series.pdf) |
 | FH34SRJ24S05SH99 | [Component Search Engine](https://componentsearchengine.com/part-view/FH34SRJ-24S-0.5SH(99)/Hirose) | [Datasheet](https://www.hirose.com/en/product/document?clcode=CL0580-1255-6-99&productname=FH34SRJ-24S-0.5SH(99)&series=FH34SRJ&documenttype=2DDrawing&lang=en&documentid=0000990903) |
 | MAX17048G+T10 | [SnapMagic](https://www.snapeda.com/parts/MAX17048G+T10/Analog+Devices/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/MAX17048G+T10/Analog%20Devices/datasheet/) |
 | MBR0530 | [Mouser](https://ro.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/40/schottky-3165252.pdf) |
 | PGB1010603MR | [SnapMagic](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse%20Inc./datasheet/) |
 | QWIIC_CONNECTORJS | [Mouse](https://eu.mouser.com/ProductDetail/Adafruit/4208?qs=PzGy0jfpSMtbScLbr0L5dw%3D%3D) | [Datasheet](https://www.youtube.com/watch?v=Z6ACqvqwDWE) |
 | SAMACSYS_PARTS_USB4110-GF-A | [Component Search Engine](https://componentsearchengine.com/part-view/USB4110-GF-A/GCT%20(GLOBAL%20CONNECTOR%20TECHNOLOGY)) | [Datasheet](https://gct.co/files/drawings/usb4110.pdf) |
 | SI1308EDL-T1-GE3 | [Component Search Engine](https://componentsearchengine.com/part-view/SI1308EDL-T1-GE3/Vishay) | [Datasheet](https://componentsearchengine.com/Datasheets/1/SI1308EDL-T1-GE3.pdf) |
 | SJ | [GrabCAD](https://grabcad.com/library/solder-jumpers-1) | [Datasheet](https://www.youtube.com/watch?v=Z6ACqvqwDWE) |
 | USBLC6-2SC6Y | [SnapMagic](https://www.snapeda.com/parts/USBLC6-2SC6Y/STMicroelectronics/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/USBLC6-2SC6Y/STMicroelectronics/datasheet/) |
 | W25Q512JVEIQ | [SnapMagic](https://www.snapeda.com/parts/W25Q512JVEIQ/Winbond+Electronics/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/W25Q512JVEIQ/Winbond%20Electronics/datasheet/) |
 | XC6220A331MR-G | [Component Search Engine](https://componentsearchengine.com/part-view/XC6220A331MR-G/Torex) | [Datasheet](https://product.torexsemi.com/system/files/series/xc6220.pdf) |

# Hardware Functionality Description

### 1. Battery 🔋
 Model: CELLEVIA BATTERIES LP584174 <br>
 Specifications: 3.7V, 1800mAh  <br>
 Functionality: It is rechargeable battery, designed for portable electronic devices. It provides a stable power supply, high energy density, and a lightweight form factor. Ideal for IoT devices, wearables, embedded systems, and battery powered applications, it ensures reliable performance with a long cycle life.

 ### 2. ESP32-C6 📡
 Model: ESP32-C6-WROOM-1 <br>
 Specifications:
  * 2.4 GHz Wi-Fi 6 (802.11 ax)
  *  Bluetooth® 5 (LE) with Long Range support
  *  Zigbee and Thread(802.15.4) for low-power mesh networking  <br>
  
  Functionality: The ESP32-C6-WROOM-1 is the central controller of the project, handling all communication, control, and processing

  ### 3. E-Paper Display 📺
  Model: 7.5inch e-Paper V2 <br>
  Specifications: resolution : 800 x 480, weight ~ 44 g <br>
  Functionality: The 7.5-inch e-Paper V2 display provides a high contrast, low power visual output suitable for battery-powered applications. Unlike traditional displays, it retains content without power, making it ideal for low energy and always on applications.

 ### 4. BME688 🌡️
 Interface: I2C <br>
 Specifications:
  * Gas Sensor: Detects volatile organic compounds, carbon monoxide, hydrogen, and other gases
  * Humidity Sensor: 0–100% RH, accuracy ±3%
  * Temperature Sensor: -40°C to 85°C, accuracy ±0.5°C
  * Pressure Sensor: 300–1100 hPa, accuracy ±0.6 hPa <br>
  
 Functionality: The BME688 is an advanced environmental sensing module, providing real-time monitoring of air quality, humidity, temperature, and pressure.

 ### 5. SD Card 💾
 Interface: SPI <br>
 Functionality: it serves as expandable storage, allowing users to store a large collection of e-books, documents, and other files beyond the device's internal memory

 ### 6. RTC ⏰
 Interface: I2C <br>
 Functionality: A real-time clock (RTC) keeps track of the correct time and date, even when the device is off. It helps manage power saving features, timestamps activities like reading progress, supports reminder functions, updates time-sensitive content, and ensures proper synchronization with other devices or platforms.

 ### 7. MCP73831T ♻️🔋
 Interface: USB-C <br>
 Functionality: The MCP73831T is a compact lithium-ion and lithium-polymer battery charger IC. It features low power consumption, precharge and fast charge modes, thermal regulation, and overvoltage protection, making it ideal for portable devices.

 ### 8. External NOR Flash 64MB 🎞️
 Interface: SPI <br>
 Functionality:  non-volatile memory storage that provides 64MB of data storage. It's commonly used in embedded systems and devices for storing firmware, code, or other critical data, offering fast read speeds and reliable data retention even without power.

 ### 9. LDO Voltage Regulator ⚡
 Functionality: voltage regulator that provides a stable output voltage with minimal difference between the input and output voltages.

 ### 10. Test Pads 📝
 Functionality: deubbing and testing outputs from certain components.

 ### 11. Qwiic ✅
 Functionality: easy addition of modules through I2C and SPI.

 # Estimated Power Consumption 🔋

 ### 1. Battery (CELLEVIA BATTERIES LP584174) 🔋
  * Its power consumption depends on the load it is powering. The maximum discharge current would be around 1.8A (1800mAh)
### 2. ESP32-C6 📡
  * Wi-Fi transmission: ~200mA
  * Idle mode: ~50mA
  * Deep sleep: ~10mA
### 3. E-Paper Display 📺
  * During content update: ~30-50mA
  * Idle (static content): ~0mA (only power used for maintaining the display)
### 4. BME688 🌡️
 * Active sensing: ~2.7mA
 * Idle mode: ~0.5mA (depends on the sleep settings)
### 5. SD Card 💾
 * Typical: ~10-15 mA
### 6. RTC ⏰
* Active mode: 1- 2 mA
### 7. MCP73831T ♻️🔋
*  Minimal power consumption
### 8. External NOR Flash 64MB 🎞️
* Active read/write: ~10-20mA
* Idle: <1mA
### 9. LDO Voltage Regulator ⚡
 * Idle mode: ~1-10mA (depends on the output load)
### 10. Test Pads 📝
* Minimal power consumption, essentially 0mA unless active signals are being tested.
### 11. Qwiic ✅
* Active communication: ~5-10mA (depends on the connected module)

# Total estimated power consumtion ( assuming wifi active) 🔋

 | 🛠 Component | Power estimation 🔋
 |-------------|--------|
 | ESP32-C6 | 200 mA |
 | E-Paper Display | 50 mA |
 | BME688 | 2.7 mA |
 | SD Card | 15 mA |
 | RTC | 2 mA |
 | External NOR Flash | 20 mA |
 | LDO Voltage Regulator | 10 mA |
 | Qwiic | 10 mA |


Total = 200mA + 50mA + 2.7mA + 15mA + 2mA + 20mA + 10mA + 10mA = 309.7mA

# Estimated battery life

**Battery life = 1800 mAh / 309.7 mA = 5.81 hours**

# ESP32-C6 Pin Usage

## Power connections 🔋
* Pin 2 ( 3V3) - provides 3.3V to the ESP32-C6
* Ground ( bottom-right pin) - provides ground connection

## Reset and Boot 🔁
* Pin 3 ( Reset) - manual reset pin
* Pin 15 ( IO/BOOT) - boot mode selection, pulled down by a 10K resistor

## I2C 📡
* Pin 8 ( INT_RTC) - interrupt signal from RTC
* Pin 16 ( RTC_RST) - reset for RTC
* Pin 18 ( I2C_PW) - power enable signal for I2C devices
* Pin 20 ( SDA) - data line for I2C comms
* Pin 21 ( SCL) - clock line for I2C comms

## SPI 🛰️
* Pin 4 ( SS_SD) - slave select for SD card
* Pin 7 ( SCK) - Serial clock used for synchronizing SPI comms
* Pin 10 ( MOSI) - Master Out Slave In, sending data to components
* Pin 11 ( EPD_CS) - chip select for e-paper display
* Pin 12 ( FLASH_CS) - chip select for flash memory
* Pin 27 ( MISO)  - Master In Slave Out, used for reading data from components

## E-Paper Display Control Signals 🖥️
* Pin 5 ( EPD_DC) - data control for E-Paper Display
* Pin 19 ( EPD_3V3_C) - enable pin for EPD power
* Pin 21 ( EPD_RST) - reset pin for E-Paper Display
* Pin 26 ( EPD_BUSY) - indicates when E-Paper Display is busy

## USB 🔌
* Pin 13 ( USB_D-) + Pin 14 ( USB_D+) - differential data lines for USB comms

## UART 🔧
* Pin 24 ( RX) - UART receive pin
* Pin 25 ( TX) - UART transmit pin

## Others ⚙️
* Pin 23 ( IO_CHANGE)  - interrupt or status for external components

# Pins explanation

* SPI (Serial Peripheral Interface) is used for high speed comms with the Flash and E-Paper Display.
* I2C low speed comms with sensor ( RTC).
* UART pins ( TX, RX) debugging and external serial comms.
* Dedicated control pins ( EPD_BUSY, EPD_DC) ensure efficient E-Paper operation.

# Final Product
 ![3D Image](Images/openBook_3D.png)
 ![Exploaded Image](Images/exploaded_viewv1.png)


   



 
 
 
  
