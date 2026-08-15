# CAN Bus Diagnostics

## Introduction

CAN Bus diagnostics is the process of identifying communication problems between electronic control units (ECUs) on a vehicle network.

A CAN communication fault can affect multiple vehicle systems, so diagnosis should begin by understanding which modules are affected and whether the problem is local or network-wide.

---

## Common Symptoms of CAN Problems

CAN-related faults may cause:

- Multiple warning lights
- Several communication DTCs
- Loss of communication with one or more ECUs
- Instrument cluster abnormalities
- Transmission-related faults
- ABS/ESC warnings
- No-start conditions
- Intermittent electrical problems

---

## Common CAN DTCs

CAN communication faults are commonly associated with **U-codes**.

Examples may include:

- U0100 – Lost Communication With ECM/PCM
- U0121 – Lost Communication With ABS Control Module
- U0140 – Lost Communication With Body Control Module

The exact code description and diagnostic procedure depend on the vehicle.

---

## First Diagnostic Step

Do not immediately replace an ECU.

First determine:

1. Which module cannot communicate?
2. Are multiple modules reporting communication faults?
3. Did the faults occur at the same time?
4. Is the problem permanent or intermittent?
5. Are other vehicle systems also affected?

This helps identify whether the problem is likely to be a module, wiring, power supply, ground, or network issue.

---

## Check Battery Voltage

Low system voltage can create multiple communication faults.

Before diagnosing the CAN network, check:

- Battery condition
- Battery voltage
- Charging system
- Main power connections
- Ground connections

A weak battery or unstable supply can produce misleading communication DTCs.

---

## Check ECU Power and Ground

An ECU that has lost power or ground may appear to have a CAN communication failure.

Check:

- Battery supply
- Ignition supply
- ECU grounds
- Fuse and relay circuits
- Voltage drop across grounds

Power and ground should be verified before condemning the communication network.

---

## CAN-H and CAN-L Inspection

Inspect the physical CAN network for:

- Broken wires
- Short circuits
- Corrosion
- Loose connectors
- Damaged terminals
- Water intrusion
- Incorrect repairs

CAN-H and CAN-L are normally routed as a twisted pair.

---

## CAN Termination Resistance

On many high-speed CAN networks, termination is provided by two resistors, commonly around **120 Ω each**, located at the physical ends of the network.

With the network powered down, measuring between CAN-H and CAN-L can often produce approximately:

**60 Ω**

because two 120 Ω resistors are connected in parallel.

Always follow the vehicle manufacturer's test procedure because network architecture can vary.

---

## Open Circuit

An open CAN wire can interrupt communication.

Possible causes include:

- Broken wire
- Damaged connector
- Loose terminal
- Corrosion
- Poor previous repair

An open circuit may affect one module or an entire section of the network depending on the network architecture.

---

## Short Circuit

CAN communication can be affected by:

- CAN-H short to ground
- CAN-L short to ground
- CAN-H short to CAN-L
- CAN wire short to battery voltage

A short can cause multiple modules to lose communication.

---

## Using an Oscilloscope

An oscilloscope can provide a more detailed view of CAN communication than a basic multimeter.

It can help identify:

- Missing communication
- Distorted signals
- Electrical interference
- Wiring problems
- Abnormal differential signalling

For advanced diagnosis, waveform analysis should be compared with known-good patterns or manufacturer specifications.

---

## Network Isolation

When multiple modules report communication faults, identify the affected network section.

A diagnostic strategy may include:

1. Identify the modules reporting faults.
2. Check the network topology.
3. Identify shared CAN wiring.
4. Check power and ground.
5. Inspect connectors.
6. Isolate the affected network section where the manufacturer's procedure allows.
7. Recheck communication.

Never disconnect modules randomly because doing so can create additional faults.

---

## Intermittent CAN Faults

Intermittent communication faults can be difficult to reproduce.

Possible causes include:

- Loose terminals
- Corrosion
- Harness movement
- Vibration
- Water intrusion
- Temperature-related faults
- Poor grounds
- Internal module faults

A technician may need to monitor the network while reproducing the customer's complaint.

---

## CAN Diagnostic Workflow

**Complaint → Scan → Identify U-Codes → Check Voltage → Check Power/Ground → Inspect Network → Test CAN-H/CAN-L → Analyze Signals → Isolate Fault → Repair → Verify**

---

## Important Diagnostic Principle

A communication DTC identifies a communication problem.

It does **not automatically identify the failed component**.

Always separate:

**Power Problem**

from

**Ground Problem**

from

**Wiring Problem**

from

**Network Problem**

from

**Module Problem**

---

## Verification After Repair

After repairing a CAN-related fault:

1. Clear relevant DTCs where appropriate.
2. Cycle the ignition.
3. Scan all relevant modules.
4. Confirm communication.
5. Check for returning U-codes.
6. Verify Live Data where applicable.
7. Perform a road test.
8. Re-scan the vehicle.

---

## CAN and Motorsport

CAN diagnostics provides a foundation for understanding vehicle data networks.

The same concepts become important in motorsport for:

- ECU communication
- Data acquisition
- Sensor data
- Powertrain monitoring
- Vehicle systems integration
- Race-car telemetry

Understanding CAN at the diagnostic level is therefore an important step toward advanced automotive data analysis and motorsport engineering.

---

## Arvix Auto Expert

Automotive Diagnostics • ECU Systems • CAN Bus • Vehicle Technology • Motorsport Engineering
