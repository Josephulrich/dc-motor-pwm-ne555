# 12 V DC Motor Speed Control with NE555 (PWM)

![schema_ne555_motor](hardware/schematics/schema_ne555_motor.png)

![PCB, top view](hardware/pcb/pcb_top.png)

## Objective

Control the speed of a 12 V DC motor with a potentiometer, by generating a PWM signal with an NE555 in astable mode.

## Operating Principle

- The NE555 is configured in astable mode to generate a PWM signal.
- A potentiometer adjusts the PWM duty cycle.
- An IRFZ44N MOSFET switches the motor according to the PWM signal.
- A freewheeling diode protects the circuit against inductive voltage spikes.

## Schematic

The schematic below shows:

- The NE555 (U1) in astable mode.
- The potentiometer PV1 used to set the duty cycle.
- The MOSFET Q1 (IRFZ44N) and the diode D1 (1N4007).

![Detailed schematic](hardware/schematics/schema_ne555_motor.png)

## PCB

PCB designed in Altium Designer.

![PCB, top view](hardware/pcb/pcb_top.png)

## Build and Results

- Prototype built and tested on the bench.
- Speed adjustment through the potentiometer validated.

## Possible Improvements

- Add a speed display (potentiometer + ADC + microcontroller).
- Add overcurrent protection.
- Replace the 1N4007 with a fast-recovery or Schottky diode, better suited to PWM switching.
- 3D-printed enclosure.

## Project Files

- `hardware/schematics/`: electrical schematics.
- `hardware/pcb/`: PCB files and exports.
- `assets/photos/`: photos of the build.
- `docs/`: notes, calculations, simulations.

## Author

**Joseph Mbode**

Embedded systems engineer, electronics and PCB design.

- LinkedIn: [Joseph Mbode](https://www.linkedin.com/in/joseph-mbode)
- GitHub: [@Josephulrich](https://github.com/Josephulrich)
