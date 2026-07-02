# LoRa Puck

## About the Project

This project is a LoRa Puck designed using EasyEDA.

The main purpose of this project was to learn how to design an embedded hardware circuit from scratch. Instead of directly working on the PCB, I first focused on creating a complete and properly connected schematic.

The design is built around the Raspberry Pi RP2040 microcontroller and the SX1262 LoRa transceiver. It also includes the required power supply, USB interface, clock circuit, and supporting components needed for the board to work properly.

This project helped me understand how different electronic components are connected together before moving to PCB design. :contentReference[oaicite:0]{index=0}

---

## Tools Used

- EasyEDA
- JLCPCB Component Library

---

## Main Components

- Raspberry Pi RP2040
- SX1262 LoRa Transceiver
- USB Type-C Connector
- AP2112 3.3V Voltage Regulator
- 32 MHz Crystal
- RF Switch
- Inductors
- Capacitors
- Resistors

---

## What I Did

### 1. Created a New Project

I started a new project in EasyEDA and created a blank schematic page.

---

### 2. Selected the Components

I searched for all the required components from the EasyEDA library and placed them on the schematic.

The main components include:

- RP2040 Microcontroller
- SX1262 LoRa Transceiver
- USB Type-C Connector
- Voltage Regulator
- Crystal Oscillator

---

### 3. Built the Power Circuit

I added the voltage regulator along with capacitors to provide a stable 3.3V supply for the board.

---

### 4. Connected the RP2040

The RP2040 was placed at the center of the design, and all the required GPIO, SPI, USB, power, and reset connections were added.

---

### 5. Connected the LoRa Module

The SX1262 LoRa transceiver was connected to the RP2040 using SPI communication.

I also connected the required control pins like:

- NSS
- MISO
- MOSI
- SCK
- BUSY
- DIO1
- RESET

---

### 6. Added the Clock Circuit

A 32 MHz crystal oscillator with the required capacitors was connected to provide the clock signal for the LoRa transceiver.

---

### 7. Added the RF Section

The RF switch, matching components, inductors, and capacitors were connected between the LoRa transceiver and the antenna path.

---

### 8. Connected the USB Interface

A USB Type-C connector was added for power and USB communication with the RP2040.

---

## What I Learned

Through this project, I learned:

- How to use EasyEDA
- How to create an electronic schematic
- How to select the required components
- How to connect a microcontroller with a LoRa transceiver
- Basic power supply design
- USB interface connections
- RF circuit basics
- Importance of checking schematic connections before PCB design

This project gave me practical experience in understanding how a complete embedded hardware circuit is designed before creating the PCB.

---

## Project Structure

```text
LoRa-Puck/
│
├── Schematic
└── README.md
```


**Manish Vanjari**


GitHub: [https://github.com/Manish-Datrik](https://github.com/Manish-Datrik/LoRa-Puck.git)
