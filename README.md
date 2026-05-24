# Distance-Controlled Sound Generator Arduino

A simple Arduino Uno mini-keyboard project that generates sounds using push buttons and an HC-SR04 ultrasonic sensor. The system can also record and playback short sound sequences.

---

# Project Preview

## Breadboard View

![Breadboard View](images/breadboard.png)

## Circuit Schematic

![Circuit Schematic](images/schematic.png)

---

# Features

- 3 sound outputs (speakers/buzzers)
- Ultrasonic distance-controlled sound generation
- Manual button-controlled notes
- Sound sequence recording and playback
- LED indicators
- UART distance monitoring
- Hardware and software PWM

---

# How It Works

The HC-SR04 ultrasonic sensor measures the distance to an object and activates specific speakers and LEDs.

| Distance | Action |
|---|---|
| 0–10 cm | All speakers and LEDs active |
| 10–20 cm | Speaker 1 + LED1 active |
| 20–30 cm | Speaker 2 + LED2 active |
| 30–40 cm | Speaker 3 + LED3 active |
| >40 cm | Everything disabled |

The user can also manually play notes using buttons.

---

# Components Used

| Quantity | Component |
|---|---|
| 1 | Arduino Uno R3 |
| 1 | HC-SR04 Ultrasonic Sensor |
| 3 | Speakers / Buzzers |
| 5 | Push Buttons |
| 3 | LEDs |
| 3 | 1 kΩ Resistors |
| 3 | 10 kΩ Resistors |
| 1 | Breadboard |
| Several | Jumper Wires |

---

# Pin Configuration

| Component | Pin |
|---|---|
| Note 1 | PD2 |
| Note 2 | PD3 |
| Note 3 | PD4 |
| RECORD Button | PC1 |
| PLAY Button | PC2 |
| Speaker 1 | PB1 |
| Speaker 2 | PD5 |
| Speaker 3 | PB3 |
| LED1 | PB4 |
| LED2 | PB5 |
| LED3 | PD7 |
| HC-SR04 TRIG | PC0 |
| HC-SR04 ECHO | PB0 |

---

# How to Run

1. Build the circuit according to the schematic.
2. Upload the code to Arduino Uno.
3. Open Serial Monitor at:

```text
9600 baud
```

4. Use buttons or the ultrasonic sensor to generate sounds.
5. Press RECORD to start recording.
6. Press PLAY to replay the recorded sequence.

---

# Technologies Used

- AVR C
- Arduino Uno
- UART Communication
- Hardware PWM
- Software PWM
- HC-SR04 Ultrasonic Sensor

---

# Author
Miłosz Jabłoński
