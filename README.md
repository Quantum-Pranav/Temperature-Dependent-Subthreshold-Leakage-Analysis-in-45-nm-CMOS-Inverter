# Temperature-Dependent-Subthreshold-Leakage-Analysis-in-45-nm-CMOS-Inverter



This repository presents a DC simulation study of subthreshold leakage current and static power variation with temperature in a 45 nm CMOS inverter.

## Overview
As CMOS technology scales, OFF-state leakage becomes an important contributor to standby power.  
This project analyzes how subthreshold leakage current and static power change with temperature for a single, minimum-size CMOS inverter.

## Methodology
- Technology: 45 nm CMOS (GPDK)
- Device type: Nominal-Vth 1 V core devices
- Supply voltage (VDD): 1.0 V
- Analysis: DC operating-point analysis
- Temperature range: 0 °C to 100 °C
- Measured quantity: Supply current (IDD) and static power (VDD × IDD)

The inverter output was left floating to isolate static leakage effects.

## Circuit Schematic
![CMOS Inverter Schematic](results/inverter_schematic.png)

## Results

### Leakage Current vs Temperature
![Leakage Current vs Temperature](results/leakage_current_vs_temperature.png)

- OFF-state leakage increased from ~15 pA at 25 °C to ~38 pA at 100 °C.
- The monotonic increase reflects temperature-dependent subthreshold conduction.

### Static Power vs Temperature
![Static Power vs Temperature](results/static_power_vs_temperature.png)

- Static power increased from ~15 pW to ~38 pW with temperature.
- The trend confirms exponential leakage behavior under standby conditions.

## Key Takeaway
Although the absolute leakage per inverter is small, its exponential temperature dependence and linear scaling with gate count make it a critical factor in standby power for scaled CMOS technologies.

## Tools Used
- Cadence Virtuoso ADE (Spectre)
- GPDK 45 nm
