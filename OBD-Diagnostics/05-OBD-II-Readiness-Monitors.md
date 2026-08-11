# OBD-II Readiness Monitors

## What is an OBD-II Readiness Monitor?

An OBD-II readiness monitor is a self-test performed by the vehicle's ECU to check whether specific emission-related systems are working correctly.

These monitors help determine whether the vehicle's emission control systems have completed their required diagnostic tests.

---

## Why is Readiness Important?

Readiness status is useful for:

- Emission testing
- Vehicle inspection
- Used-car diagnosis
- Detecting incomplete diagnostic cycles
- Verifying repairs after clearing DTCs

---

## Common Readiness Monitors

Typical OBD-II monitors include:

- Misfire Monitor
- Fuel System Monitor
- Comprehensive Components Monitor
- Oxygen Sensor Monitor
- Oxygen Sensor Heater Monitor
- EGR System Monitor
- EVAP System Monitor
- Catalyst Monitor

The exact monitors available depend on the vehicle and engine configuration.

---

## Ready vs Not Ready

### READY

The ECU has completed the required self-test for that monitor.

### NOT READY

The ECU has not yet completed the required test.

This can happen after:

- Battery disconnection
- DTC clearing
- ECU reset
- Recent repairs
- Insufficient driving conditions

---

## Important Diagnostic Point

Clearing DTCs does not repair the problem.

When DTCs are cleared, the readiness monitors may also become incomplete.

The vehicle must usually be driven through the required conditions so the ECU can run its self-tests again.

---

## Example

A vehicle has an EVAP-related fault.

After repairing the fault:

1. Repair the root cause
2. Clear the DTC
3. Check readiness monitors
4. Perform the required drive cycle
5. Recheck readiness
6. Confirm that the system has completed its test
7. Verify that no DTC returns

---

## Diagnostic Principle

**Never assume that a vehicle is fully diagnosed just because the MIL is OFF.**

Always check:

- Stored DTCs
- Pending DTCs
- Readiness monitors
- Live data
- Freeze-frame data
- Vehicle symptoms

---

## Arvix Auto Expert

Automotive Diagnostics • Vehicle Inspection • OBD & Automotive Technology
