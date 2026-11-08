# Alekya – Construction Robot

**Alekya** is a modular construction automation system built from standard, open-source 3D printer and CNC hardware (NEMA 17 stepper motors, linear rails, belts, endstops and G-code). The goal is to automate basic building work such as **placing bricks** and **extruding mortar**, using parts anyone can print and buy.

> Status: early prototype (2019). Shared as-is so others can learn from it and build on it.

## What's in this repository

| Folder / file | What it is |
|---|---|
| `3d models used in Alekya/` | 3D-printable parts (STL files) used to build the machine |
| `gcode/brick-dispenser.gcode` | G-code that picks and places bricks using the brick dispenser tool |
| `gcode/mortar-extruder-toilet-booth.gcode` | G-code that extrudes mortar for a small toilet-booth structure |
| `LICENSE` | GPL-3.0 open-source license |

## Main 3D-printed parts

- **Motion:** linear rail, linear rail support, bearing flange, bearing idler, belt tensioners, coupling, gears
- **Z axis:** Z holders, Z axis nut holder, Z nut
- **Sensors:** endstop holder, inductive sensor holder
- **Brick tool:** brick dispenser holder, "bd glove" and glove gear
- **Mortar tool:** syringe holder, syringe holder cap, syringe plunger, NEMA 17 syringe motor holder
- **Other:** pipe flange, end cones

## How it works (overview)

1. The machine is a gantry (like a large 3D printer or CNC) that moves in X, Y and Z.
2. A **brick dispenser** tool, driven by servo commands (`M280`), grips and places bricks at set positions.
3. A **syringe-style mortar extruder**, driven by a NEMA 17 motor, lays mortar along the wall path.
4. Each job is a plain G-code file, so it can run on common 3D-printer / CNC firmware.

## Photos

_Coming soon._

## License

This project is open source under the [GNU GPL v3.0](LICENSE). You are free to use, change and share it, as long as your changes stay open source under the same license.
