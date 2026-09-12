**16-Bit Hardware Snake and Ladders Digital Logic Game**

**Overview**

A microcontroller-free, two-player 16-bit Snake and Ladders game designed, simulated, and laid out for PCB production in Proteus Design Suite. Built strictly with discrete digital logic components, the system features customizable board coordinates, a 555 timer electronic dice generator, multi-channel player tracking, and automatic victory detection.

**Project Demonstration**

[Software Simulation & Overview on YouTube](https://youtu.be/vfKOnuiyQQE?si=-LveDh7Ymb3cpJRm)

**Key Features**

* **Discrete Logic Architecture:** Built entirely without microcontrollers using standard ICs.
* **16-State Board Grid:** Manages positional state across a 16-step matrix for two players.
* **Configurable Board Settings:** Manual hardware switches set snake (head/tail) and ladder (base/top) coordinates prior to play.
* **555 Timer Electronic Dice:** An astable multivibrator circuit generates unbiased roll counts frozen via user button press.
* **Automatic Victory Detection:** Win-logic freezes gameplay and activates an indicator upon reaching state 16.
* **Proteus Assets:** Complete simulation schematics and production-ready PCB layouts included.

**Hardware Logic Overview**

* **Priority Encoders:** Detect snake heads and ladder bases to execute instant conditional jumps.
* **Multiplexers (MUXs):** Manage turn-toggling and data bus routing between Player 1 and Player 2.
* **Decoders:** Translate binary state data to drive visual state outputs.
* **Logic Gates:** Handle positional arithmetic, boundary validation, and state latching.

**Repository Structure**

* **Schematics/** – Proteus simulation schematics (`.pdsprj`)
* **PCB/** – Proteus PCB layout design files
* **README.md** – Project documentation

**Simulation Instructions**

1. Open the project file in **Proteus Design Suite (v8.0+)**.
2. Set snake and ladder start/end coordinates using the onboard switch matrix.
3. Run the simulation and use the **Dice Roll** button to initiate turns.
