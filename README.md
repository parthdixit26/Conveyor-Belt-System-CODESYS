# Conveyor Belt System — CODESYS V3.5

## Overview
A PLC program simulating an industrial conveyor belt system 
with three sensor positions and an automated paint station. 
Programmed in CODESYS V3.5 SP22 using Ladder Logic (LD).

## System Layout
The conveyor belt moves objects across three sensor positions:
- **Position A (Sensor A)** — detects object entering the belt
- **Position B (Sensor B)** — triggers the paint station
- **Position C (Sensor C)** — detects object leaving the belt

A paint unit is mounted above Position B and activates 
automatically when an object is detected by Sensor B.

## Features
- Start/Stop control via green/red indicator lights
- Automatic paint activation at Position B
- Three position sensors (A, B, C) for object tracking
- Conveyor motor control based on system state

## Inputs
| Variable | Type | Description |
|---|---|---|
| Start | BOOL | Starts the conveyor belt |
| Stop | BOOL | Stops the conveyor belt |
| Sensor_A | BOOL | Object detected at Position A |
| Sensor_B | BOOL | Object detected at Position B |
| Sensor_C | BOOL | Object detected at Position C |

## Outputs
| Variable | Type | Description |
|---|---|---|
| ConveyorMotor | BOOL | Conveyor belt motor running |
| PaintStation | BOOL | Paint unit activated |
| GreenLight | BOOL | System running indicator |
| RedLight | BOOL | System stopped indicator |

## Languages Used
- Ladder Logic (LD)

## How to Open
1. Install CODESYS V3.5 SP22 or later (free from codesys.com)
2. Download all project files and keep them in the same folder
3. Open the .project file in CODESYS
4. Run in Simulation Mode: Online → Simulation Mode → Login → Start


## Author
Parth — Electronics Engineering Master's Student  
Berlin, Germany
