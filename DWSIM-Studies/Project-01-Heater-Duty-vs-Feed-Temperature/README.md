# Project 01: Heat Recovery and Heater Duty Analysis using DWSIM

## Objective

This project investigates how process conditions affect heater energy consumption and heat recovery performance using DWSIM.

The study focuses on three questions:

1. How does feed temperature affect heater duty?
2. How does heat exchanger area affect heat recovery?
3. How does hot stream temperature affect utility consumption?

---

## Software

* DWSIM 9.0.5
* Property Package: Peng-Robinson
* Working Fluid: Water

---

## Process Configuration

Feed Stream → Heat Exchanger → Heater → Product Stream

A hot utility stream was introduced to recover heat before the feed entered the heater.

---

## Study 1: Effect of Feed Temperature on Heater Duty

The feed temperature was varied while maintaining a product temperature of 80°C.

### Results

| Feed Temperature (°C) | Heater Duty (kW) |
| --------------------- | ---------------- |
| 25                    | 68.998           |
| 35                    | 56.483           |
| 45                    | 43.965           |
| 55                    | 31.436           |
| 65                    | 18.886           |

### Observation

Heater duty decreased approximately linearly as feed temperature increased.

This behavior follows the energy balance equation:

Q = mCp(Tout − Tin)

A higher feed temperature reduces the required temperature rise across the heater, resulting in lower energy consumption.

---

## Study 2: Effect of Heat Exchanger Area

The heat exchanger area was increased while keeping process conditions unchanged.

### Key Findings

* Larger heat exchanger area increased heat recovery.
* Heater duty decreased significantly.
* Phase change warnings appeared at large heat transfer areas.
* The outlet temperature approached the boiling point of water (~100°C).

---

## Study 3: Effect of Hot Stream Temperature

The hot stream temperature was varied to determine the minimum temperature required to eliminate heater duty.

### Results

The heater duty approached zero when the hot stream temperature was approximately 143–144°C.

### Engineering Interpretation

At this condition, the heat exchanger alone supplied nearly all thermal energy required by the process.

This demonstrates the concept of heat integration and utility reduction used in industrial process design.

---

## Lessons Learned

Through this project, I explored:

* Energy balances
* Sensible heat transfer
* Heat exchanger performance
* Heat recovery
* Utility reduction
* Sensitivity analysis
* Process optimization

This project was completed as part of my self-study in process simulation and chemical engineering process analysis.
