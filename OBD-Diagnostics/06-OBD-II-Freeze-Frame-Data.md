# OBD-II Freeze Frame Data

## What is Freeze Frame Data?

Freeze Frame Data is a snapshot of vehicle operating conditions recorded by the ECU when certain diagnostic trouble codes are detected.

It helps a technician understand what the vehicle was doing when the fault occurred.

---

## Why is Freeze Frame Important?

A DTC tells us what type of fault was detected.

Freeze Frame helps answer:

**"Under what conditions did the fault occur?"**

It can help identify whether the problem occurred during:

- Cold start
- Engine idle
- Acceleration
- Cruising
- High engine load
- High engine temperature

---

## Common Freeze Frame Parameters

Depending on the vehicle, Freeze Frame may contain:

- Engine RPM
- Vehicle Speed
- Engine Coolant Temperature
- Engine Load
- Throttle Position
- Fuel Trim
- Intake Air Temperature
- MAF
- MAP
- Fuel System Status

The available parameters vary by vehicle and ECU.

---

## Example

Suppose the vehicle stores:

**P0171 – System Too Lean**

Freeze Frame shows:

- Engine RPM: 750 RPM
- Engine Coolant Temperature: 88°C
- Engine Load: Low
- STFT: +22%
- LTFT: +18%

This information suggests that the ECU was making significant positive fuel corrections when the fault was detected.

The technician can then investigate possible causes such as:

- Vacuum leak
- Unmetered air
- Low fuel pressure
- MAF measurement error
- Injector problem

Freeze Frame does not prove the root cause. It provides diagnostic evidence.

---

## Freeze Frame vs Live Data

### Freeze Frame

Shows the conditions recorded when the fault occurred.

### Live Data

Shows the vehicle's current operating conditions.

Using both together can provide much stronger diagnostic information.

---

## Diagnostic Workflow

When a DTC is found:

1. Record the DTC.
2. Save Freeze Frame Data.
3. Check current Live Data.
4. Compare the two.
5. Reproduce the symptom if possible.
6. Test the related system.
7. Identify the root cause.
8. Repair the vehicle.
9. Verify the repair.

---

## Important Diagnostic Principle

Do not clear DTCs before recording useful diagnostic information.

Clearing codes can remove valuable Freeze Frame information on some vehicles.

Always capture relevant data before performing a reset or clearing procedure.

---

## Professional Approach

A good technician does not diagnose from the DTC alone.

A stronger diagnosis combines:

**DTC + Freeze Frame + Live Data + Symptoms + Physical/Electrical Tests**

This approach helps reduce unnecessary parts replacement and improves diagnostic accuracy.

---

## Arvix Auto Expert

Automotive Diagnostics • Vehicle Inspection • OBD & Automotive Technology
