# ⚗️ Reaction Kinetics Simulator

A Python tool for simulating chemical reaction kinetics using numerical integration methods (Euler and Runge-Kutta 4th order). Designed for scientific computing applications in chemistry.

## Features

- **Simple reactions**: A → B with 0th, 1st, or 2nd order kinetics
- **Reversible reactions**: A ⇌ B with forward and reverse rate constants
- **Consecutive reactions**: A → B → C (intermediate buildup/decay)
- **Arrhenius equation**: Rate constant vs temperature plots
- **Numerical methods**: Both Euler and RK4 integration available
- **Data export**: CSV output for downstream analysis
- **Visualization**: matplotlib plots of concentration vs time

## Installation

```bash
pip install matplotlib
```

## Usage

```bash
python reaction_kinetics.py
```

## Example Output — Consecutive Reactions A → B → C

```
k1 = 0.3 s⁻¹ (A → B)
k2 = 0.1 s⁻¹ (B → C)
```

The simulator captures the classic intermediate peak of B before it converts to C.

## Scientific Background

| Concept | Formula |
|--------|---------|
| 1st Order Rate | `d[A]/dt = -k[A]` |
| Reversible Eq | `d[A]/dt = -kf[A] + kr[B]` |
| Arrhenius | `k = A·exp(-Ea/RT)` |
| RK4 Integration | 4th-order accuracy, stable for stiff systems |

## Applications

- Modeling enzyme kinetics
- Simulating drug degradation
- Teaching reaction mechanism concepts
- Validating experimental kinetics data

## Author
Tejeswara Rao Guttavalli
