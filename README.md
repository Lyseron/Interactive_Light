# Interactive Light

Interactive Light is an Arduino-based prototype that controls a light depending on movement or presence.

The idea is to create a soft interactive lighting system that reacts when someone gets close to or moves away from a specific area, such as a bed, a desk, or a room entrance.

This project was made as a physical prototype to explore electronics, sensors, light control, and real-world interaction through code.

## Project idea

The goal of this project is to make a light react progressively instead of using a simple ON/OFF switch.

For example:

* when someone approaches the bed, the light can slowly turn off
* when someone gets up or moves away, the light can gradually turn back on
* the brightness changes smoothly to create a more natural interaction

This project combines Arduino programming, basic electronics, and interactive object design.

## Demo

### Prototype

<p align="center">
  <img src="assets/prototype-front.jpg" width="300" alt="Interactive Light prototype front view">
  <img src="assets/circuit.jpg" width="300" alt="Arduino circuit">
</p>

### Video demonstration

<p align="center">
  <video src="assets/demo.mp4" width="500" controls></video>
</p>

### Final result

<p align="center">
  <img src="assets/result.jpg" width="500" alt="Interactive Light final result">
</p>

## How it works

The project uses an Arduino board connected to a sensor and a light source.

The sensor detects movement or presence.
The Arduino reads the sensor value and adjusts the light intensity using PWM.

Instead of switching the light instantly on or off, the brightness changes progressively to create a smoother and softer effect.

## Components

| Component                 | Role                                |
| ------------------------- | ----------------------------------- |
| Arduino board             | Controls the project logic          |
| Distance or motion sensor | Detects presence or movement        |
| LED or light module       | Produces the light                  |
| Resistors                 | Protect the components              |
| Breadboard                | Used to build the prototype circuit |
| Jumper wires              | Connect the components together     |

## Features

* Detects movement or presence
* Controls light intensity
* Uses progressive brightness changes
* Creates a soft fade effect
* Works as a simple physical prototype
* Combines code and electronics
* Explores real-world interaction

## Code logic

The program follows a simple logic:

```txt
read sensor value
↓
check if someone is close or moving
↓
adjust brightness
↓
apply smooth fade effect
↓
update the light
```

The light intensity is controlled with PWM, which allows the LED brightness to change gradually.

## Possible structure

```txt
Interactive-Light/
├── README.md
├── interactive_light.ino
└── assets/
    ├── prototype-front.jpg
    ├── circuit.jpg
    ├── demo.mp4
    └── result.jpg
```

## Installation

Open the Arduino file in the Arduino IDE:

```txt
interactive_light.ino
```

Connect the Arduino board to your computer, select the correct board and port, then upload the code.

## Usage

Once the code is uploaded:

1. Power the Arduino.
2. Place the sensor near the area you want to detect.
3. Move closer or farther from the sensor.
4. The light reacts by changing its brightness progressively.

## Possible improvements

This project can be improved by adding:

* a smoother fade effect
* multiple LEDs
* different lighting modes
* a better physical enclosure
* a more precise sensor
* automatic calibration
* a button to change modes
* a mobile app or remote control

## Skills practiced

* Arduino programming
* Basic electronics
* Sensors
* PWM output
* LED control
* Breadboard prototyping
* Physical computing
* Interactive object design
* Hardware debugging
* Connecting code with real-world behavior

## What I learned

This project helped me understand how software can interact with physical components.

I practiced reading sensor values, controlling an output, wiring electronic components, and thinking about how a user interacts with a physical object.

It also helped me explore the connection between programming, electronics, and creative prototyping.

## Notes

This project is a prototype and can be adapted depending on the sensor and light source used.

The main goal was to explore interactive lighting and learn how to combine code, electronics, and user interaction.
