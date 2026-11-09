# 🌈 Raspberry Pi 4 – RGB LED Blinking Project

A beginner-friendly electronics and Python project using **Raspberry Pi 4 Model B** to control an RGB LED through GPIO pins. The project demonstrates GPIO output control, colour mixing, and basic hardware programming using Python.

## 📌 Project Overview

This project uses a Raspberry Pi 4 to control an RGB LED and generate different colours by controlling its Red, Green, and Blue channels.

By changing the HIGH and LOW states of the GPIO pins, the Raspberry Pi can produce different lighting combinations.

### ✨ Features

- Control an RGB LED using Raspberry Pi GPIO.
- Generate different colours using RGB combinations.
- Programmed using Python.
- Simple and beginner-friendly hardware setup.
- Demonstrates GPIO interfacing and digital output control.

## 🛠️ Hardware Requirements

| Component | Quantity |
|---|---:|
| Raspberry Pi 4 Model B | 1 |
| RGB LED | 1 |
| 220Ω resistors | 3 |
| Breadboard | 1 |
| Jumper wires | As required |
| Power supply for Raspberry Pi | 1 |

## 💻 Software Requirements

- Raspberry Pi OS
- Python 3
- RPi.GPIO library
- SSH terminal or Raspberry Pi terminal

## 🔌 Circuit Connections

The RGB LED has four terminals:

- Red (R)
- Green (G)
- Blue (B)
- Common terminal (Cathode or Anode)

### GPIO Connections

| RGB LED Channel | Raspberry Pi GPIO (BCM) | Physical Pin |
|---|---:|---:|
| Red | GPIO17 | 11 |
| Green | GPIO27 | 13 |
| Blue | GPIO22 | 15 |
| Common Cathode | GND | 6 |

**Note:** This pin mapping assumes a common-cathode RGB LED. Use a separate 220Ω resistor for each colour channel. For a common-anode LED, the wiring and GPIO logic must be adjusted.

## 📂 Project Structure

```text
Raspberry-Pi-RGB-LED/
│
├── main.py
├── README.md
└── requirements.txt
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project directory

```bash
cd Raspberry-Pi-RGB-LED
```

### 3. Install the GPIO library

```bash
sudo apt update
sudo apt install python3-rpi.gpio
```

### 4. Run the Python program

```bash
sudo python3 main.py
```

## 🎨 Working Principle

An RGB LED contains three individual LEDs: Red, Green, and Blue.

By controlling each channel independently, different colours can be generated.

| Red | Green | Blue | Output Colour |
|---|---|---|---|
| ON | OFF | OFF | 🔴 Red |
| OFF | ON | OFF | 🟢 Green |
| OFF | OFF | ON | 🔵 Blue |
| ON | ON | OFF | 🟡 Yellow |
| ON | OFF | ON | 🟣 Magenta |
| OFF | ON | ON | 🔵 Cyan |
| ON | ON | ON | ⚪ White |
| OFF | OFF | OFF | ⚫ OFF |

## 🧠 Concepts Learned

Through this project, the following concepts are explored:

- Raspberry Pi GPIO programming.
- Python hardware interfacing.
- Digital input and output.
- RGB colour mixing.
- Electronic circuit connections.
- Linux command-line operations.
- Running Python scripts through SSH.

## 🚀 Future Improvements

Some possible upgrades for this project:

- Smooth RGB colour transitions using PWM.
- Random colour generation.
- RGB LED patterns and animations.
- Web-based RGB LED control using Flask.
- Smartphone-based LED control.
- Integration with a Raspberry Pi home automation dashboard.

## ⚠️ Safety Precautions

- Always use current-limiting resistors.
- Never apply 5V directly to Raspberry Pi GPIO pins.
- Verify LED polarity before powering the circuit.
- Disconnect power before modifying circuit connections.

## 👨‍💻 Author

**Your Name**

Electronics | Python | Raspberry Pi | IoT | Hardware Programming

---

⭐ If you find this project useful, consider giving this repository a star!
