# PCB Fabrication for Electrocardiogram (ECG)
## Electrocardiography
An electrocardiogram (ECG or EKG) is a test designed to record the electrical signals in the heart. The ECG works by detecting the change in the electrical activity of the heart through small plastic patches placed on specific spots on the chest, arms and legs, known as electrodes and are connected to the ECG machine using lead wires. 

## ECG Instrumentation

ECG signals are weak (±5 mV, 0.1–150 Hz for adults, up to ~250 Hz for children) and require amplification and noise filtering for accurate readings.

### Key Components

- **Instrumentation Amplifier** — High input impedance, low output impedance, gain >1000, high CMRR. Built from multiple op-amps to safely amplify millivolt-level biosignals.
- **Filtering** — Analog (passive/active) and digital low-pass filters remove high-frequency noise outside the ECG bandwidth.
- **Driven Right Leg (DRL) Circuit** — Actively cancels common-mode noise (e.g., 60 Hz powerline interference) by injecting an inverted feedback signal through the right leg electrode, improving signal clarity and patient safety.

### Common-Mode Noise Mitigation

1. Differential amplification
2. Grounding and shielding
3. Notch filtering
4. Isolation
