# CAN Bus Waveform Analysis

## Introduction

Controller Area Network (CAN) is one of the most important communication systems used in modern vehicles.

ECUs use CAN to exchange information such as:

- Engine speed
- Vehicle speed
- Torque requests
- Sensor information
- Transmission status
- ABS information
- Body-system data

An oscilloscope can be used to observe the electrical CAN waveform and evaluate the physical communication layer.

---

## CAN-H and CAN-L

High-speed CAN generally uses two communication lines:

- CAN-H
- CAN-L

CAN uses differential signalling.

The two signals change in opposite directions during a dominant state.

This allows the network to be more resistant to electrical interference.

---

## Dominant and Recessive States

CAN communication uses two logical states:

### Recessive

The CAN-H and CAN-L lines move toward approximately the same common voltage level.

### Dominant

The voltage difference between CAN-H and CAN-L increases.

The exact voltage levels depend on the CAN implementation and vehicle architecture.

Always use manufacturer or network-specific specifications where available.

---

## Typical High-Speed CAN Behaviour

A common high-speed CAN network operates around:

**500 kbit/s**

However, vehicles may use different CAN speeds depending on the network.

Examples can include:

- 125 kbit/s
- 250 kbit/s
- 500 kbit/s
- 1 Mbit/s

Never assume the bus speed without verifying the specific network.

---

## CAN Waveform

An oscilloscope can display:

**CAN-H**

and

**CAN-L**

simultaneously.

A healthy differential waveform should show a consistent relationship between the two signals.

The exact waveform depends on:

- Transceiver design
- Network speed
- Bus loading
- Wiring
- Vehicle architecture
- Measurement setup

---

## What to Look For

When analyzing a CAN waveform, inspect:

### Voltage Levels

Are CAN-H and CAN-L reaching the expected levels?

### Symmetry

Do the two signals maintain the expected differential relationship?

### Noise

Are there unwanted disturbances on the signal?

### Distortion

Are edges or voltage levels abnormal?

### Missing Communication

Are expected communication events absent?

### Reflections

Are there waveform abnormalities caused by network wiring or termination problems?

---

## CAN Termination

Many high-speed CAN networks use termination resistors at the ends of the bus.

A common arrangement uses:

**120 Ω + 120 Ω**

which results in approximately:

**60 Ω**

when measured across CAN-H and CAN-L with the network powered down and the network topology appropriate for that test.

The actual network architecture must always be verified before applying this test.

---

## CAN Wiring Problems

Possible physical-layer problems include:

- Open CAN-H
- Open CAN-L
- CAN-H short to ground
- CAN-L short to ground
- CAN-H short to CAN-L
- Short to battery voltage
- High resistance
- Poor connectors
- Corrosion
- Incorrect repairs
- Poor termination

These problems can affect communication between multiple ECUs.

---

## Using an Oscilloscope

A basic two-channel setup can be used to observe:

**Channel 1 → CAN-H**

**Channel 2 → CAN-L**

The oscilloscope can then display both signals simultaneously.

This allows comparison of:

- Voltage
- Timing
- Differential behaviour
- Noise
- Signal distortion

The probing method must be appropriate for the vehicle and measurement equipment.

---

## Differential Signal Analysis

A useful advanced concept is:

**CAN Differential Voltage = CAN-H − CAN-L**

The differential voltage is the important electrical relationship used by the CAN transceiver to distinguish communication states.

A differential probe or suitable oscilloscope setup can provide more advanced analysis.

---

## Example Diagnostic Scenario

### Complaint

Multiple warning lights appear and several ECUs report communication faults.

### Diagnostic Approach

1. Perform a complete vehicle scan.
2. Identify all communication-related DTCs.
3. Determine which modules are unavailable.
4. Check battery voltage.
5. Check ECU power and grounds.
6. Identify the affected CAN network.
7. Inspect CAN-H and CAN-L wiring.
8. Check network termination where applicable.
9. Capture CAN-H and CAN-L waveforms.
10. Look for abnormal voltage, noise, distortion, or missing communication.
11. Isolate the affected network section.
12. Repair the physical-layer fault.
13. Recheck the waveform.
14. Confirm ECU communication.
15. Clear relevant DTCs and verify the repair.

---

## CAN Waveform vs CAN Data

It is important to distinguish between:

### Physical Layer

The oscilloscope shows the electrical waveform.

It helps diagnose:

- Wiring
- Signal integrity
- Noise
- Termination
- Transceiver behaviour

### Data Layer

A CAN analyzer or suitable diagnostic equipment can decode:

- CAN IDs
- Data bytes
- Message frequency
- Signals
- Counters
- Network traffic

The two approaches complement each other.

---

## Oscilloscope vs CAN Analyzer

### Oscilloscope

Best for:

- Electrical waveform
- Signal integrity
- Noise
- Wiring faults
- Physical-layer diagnosis

### CAN Analyzer

Best for:

- CAN IDs
- Message decoding
- Data bytes
- Message frequency
- Network traffic
- Signal interpretation

Advanced diagnostics may use both.

---

## Common Diagnostic Mistakes

Avoid:

- Assuming every CAN network uses the same speed
- Replacing an ECU based only on a U-code
- Measuring resistance on a powered network when the procedure requires power OFF
- Ignoring power and ground
- Looking at CAN-H alone
- Ignoring network topology
- Assuming a normal waveform means all CAN data is correct
- Using incorrect probing methods

---

## Professional Diagnostic Principle

**CAN communication has both a physical layer and a data layer.**

A professional diagnosis should separate:

**Power → Ground → Wiring → Physical CAN Signal → Communication → Data → ECU**

This prevents unnecessary module replacement.

---

## CAN and Advanced Vehicle Data

Understanding CAN waveform analysis creates the foundation for advanced vehicle data analysis.

The progression is:

**CAN Waveform → CAN Frames → CAN IDs → Data Bytes → Signals/PIDs → Data Logging → Telemetry**

This is an important bridge between automotive diagnostics and motorsport data engineering.

---

## Motorsport Connection

Motorsport vehicles rely heavily on electronic communication and data systems.

CAN-based data can be used for:

- ECU information
- Engine parameters
- Gearbox information
- Wheel speeds
- Temperatures
- Pressures
- Vehicle status
- Data acquisition
- Telemetry

Understanding the physical CAN layer is therefore an important foundation before moving into advanced motorsport data analysis.

---

## Arvix Auto Expert

Automotive Diagnostics • CAN Bus • Oscilloscope • ECU Communication • Vehicle Data • Motorsport Engineering
