# PCB Fabrication for Electrocardiogram (ECG)
This project involves the design, fabrication, assembly and testing of a PCB board from scratch in order to perform Electrocardiogram (ECG). The circuit response and instrumentation for each component was designed and tested on Cadence Virtuoso, and the PCB designed and assembled manually on Altium Designer. Once the PCB was fabricated, the SMD components were manually soldered and each component tested and verified using jumpers at various points in the schematic combined with oscilloscopes. 

## Introduction
### Electrocardiography
An electrocardiogram (ECG or EKG) is a test designed to record the electrical signals in the heart. The ECG works by detecting the change in the electrical activity of the heart through small plastic patches placed on specific spots on the chest, arms and legs, known as electrodes and are connected to the ECG machine using lead wires. 

### ECG Instrumentation

ECG signals are weak (±5 mV, 0.1–150 Hz for adults, up to ~250 Hz for children) and require amplification and noise filtering for accurate readings.

#### Key Components

- **Instrumentation Amplifier**: High input impedance, low output impedance, gain >1000, high CMRR. Built from multiple op-amps to safely amplify millivolt-level biosignals.
- **Filtering**: Analog (passive/active) and digital low-pass filters remove high-frequency noise outside the ECG bandwidth.
- **Driven Right Leg (DRL) Circuit**: Actively cancels common-mode noise (e.g., 60 Hz powerline interference) by injecting an inverted feedback signal through the right leg electrode, improving signal clarity and patient safety.

#### Common-Mode Noise Mitigation

- Differential amplification
- Grounding and shielding
- Notch filtering
- Isolation

## Circuit Design
### Cadence Virtuoso
<img width="600" alt="Instrumentation amplifier schematic" src="https://github.com/user-attachments/assets/fe2e838f-c249-43cc-a8b8-80fe2d44d6d4" />

*Fig. 1 — Instrumentation amplifier schematic in Cadence Virtuoso.*

<p float="left">
  <img width="400" alt="Filter stage schematic" src="https://github.com/user-attachments/assets/829fc945-e10f-4d26-9e7b-439a6d04175d" />
  <img width="400" alt="DRL circuit schematic" src="https://github.com/user-attachments/assets/85ce6e37-a367-4917-8f31-51386cb88a56" />
</p>

*Fig. 2 (left) — Input.         Fig. 3 (right) — Output.*

### PCB
<img width="600" alt="Full PCB layout" src="https://github.com/user-attachments/assets/65cffeb0-2e01-4793-b6a4-5ca772265af1" />

*Fig. 4 — Complete PCB layout in Altium Designer.*

<p float="left">
  <img width="300" alt="PCB top layer routing" src="https://github.com/user-attachments/assets/7510bc11-6ab9-47c0-a495-623f08529554" />
  <img width="300" alt="PCB bottom layer routing" src="https://github.com/user-attachments/assets/951b303b-82bc-4631-9e91-72eb2e733eac" />
</p>

*Fig. 5 (left) — Top layer routing. Fig. 6 (right) — Bottom layer routing.*

## Assembly
<img width="600" alt="Assembled PCB" src="https://github.com/user-attachments/assets/a38d2c07-ba61-4a8a-8d13-ac5f4e922bcc" />

*Fig. 7 — Assembled ECG PCB with SMD components soldered.*

## Testing











