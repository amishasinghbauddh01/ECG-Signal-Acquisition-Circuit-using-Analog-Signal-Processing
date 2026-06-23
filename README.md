# ECG Signal Acquisition Circuit

## Overview

This project presents the design and implementation of a low-cost Electrocardiogram (ECG) Signal Acquisition Circuit capable of capturing and conditioning weak cardiac electrical signals. The system employs an instrumentation amplifier, high-pass filter, low-pass filter, and 50 Hz notch filter to amplify ECG signals while minimizing noise and interference.

The project was designed, simulated, and validated through both LTspice simulations and hardware implementation.

---

## Features

- ECG signal acquisition using skin electrodes
- High-gain instrumentation amplifier for microvolt-level signals
- 50 Hz Twin-T Notch Filter for power-line noise rejection
- High-Pass Filter for baseline wander removal
- Low-Pass Filter for high-frequency noise suppression
- Analog signal conditioning for ADC integration
- LTspice simulation and hardware validation
- Low-cost biomedical instrumentation design

---

## Components Used

- UA741 Operational Amplifiers
- Resistors (10 Ω – 1 MΩ)
- Capacitors (10 nF – 100 µF)
- Ag/AgCl ECG Electrodes
- Protection Diodes
- Breadboard
- Digital Oscilloscope
- Power Supply

---

## System Architecture

ECG Electrodes
↓
Instrumentation Amplifier
↓
High-Pass Filter
↓
50 Hz Notch Filter
↓
Low-Pass Filter
↓
Output Buffer
↓
Oscilloscope / ADC / Embedded System

---

## Signal Processing Stages

### Instrumentation Amplifier

- Amplifies weak ECG signals (0.5 mV – 5 mV)
- High Common Mode Rejection Ratio (CMRR)
- Gain ≈ 900
- Noise reduction and differential signal acquisition

### High-Pass Filter

- Removes baseline wander and DC offsets
- Cutoff Frequency ≈ 0.5 Hz
- Preserves useful ECG waveform components

### Twin-T Notch Filter

- Eliminates 50 Hz power-line interference
- Notch Frequency ≈ 50 Hz
- Improved signal quality for biomedical measurements

### Low-Pass Filter

- Removes muscle artifacts and high-frequency noise
- Cutoff Frequency ≈ 150 Hz
- Preserves ECG frequency components

---

## Software & Tools Used

- LTspice
- Analog Circuit Design
- Oscilloscope Measurements
- Signal Processing Techniques

---

## Results

- Instrumentation Amplifier Gain ≈ 810–900
- Measured CMRR ≈ 91 dB
- Effective 50 Hz noise suppression
- Clean ECG waveform acquisition
- Successful hardware and simulation validation
- Suitable for ADC and embedded system integration

---

## Applications

- Biomedical Signal Processing
- ECG Monitoring Systems
- Wearable Health Devices
- Medical Electronics
- Embedded Healthcare Systems
- Academic Research & Learning

---

## Future Scope

- Digital Signal Processing (DSP)
- STM32/ESP32 Integration
- Real-Time ECG Monitoring
- Mobile Health Applications
- Cloud-Based Health Analytics
- Wearable ECG Devices

---

## License

This project is developed for academic and educational purposes.

⭐ If you found this project useful, consider giving it a star.
