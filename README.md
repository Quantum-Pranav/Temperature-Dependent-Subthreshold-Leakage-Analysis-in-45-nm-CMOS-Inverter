# Temperature-Dependent-Subthreshold-Leakage-Analysis-in-45-nm-CMOS-Inverter




This repository presents a DC simulation study of subthreshold leakage current and static power variation with temperature in a 45 nm CMOS inverter.

## Overview
As CMOS technology scales, OFF-state leakage becomes increasingly important for standby power consumption.  
This project analyzes how subthreshold leakage current and static power change with temperature for a single, minimum-size CMOS inverter.

## Methodology
- Technology: 45 nm CMOS (GPDK)
- Device type: Nominal-Vth 1 V core devices
- Supply voltage: 1.0 V
- Analysis: DC operating-point analysis
- Temperature range: 0 °C to 100 °C
- Measured quantity: Supply current (IDD) and static power (VDD × IDD)

The inverter output was left floating to isolate static leakage effects.

## Results
- OFF-state leakage current increased from ~15 pA at 25 °C to ~38 pA at 100 °C.
- Static power increased from ~15 pW to ~38 pW with temperature.
- The results show an exponential increase in leakage with temperature, consistent with weak-inversion conduction in CMOS devices.

## Files
- `circuit.png` – CMOS inverter schematic
- `leakage_current_vs_temperature.png` – Leakage current vs temperature
- `static_power_vs_temperature.png` – Static power vs temperature

## Tools Used
- Cadence Virtuoso ADE (Spectre)
- GPDK 45 nm
