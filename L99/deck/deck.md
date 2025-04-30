---
marp: true
class: invert
math: katex
---

# The Susceptible-Infected-Recovered (SIR) Model

Ella Xu
April 29, 2025

---

# Background

- Kermack & McKendrick 1927
- Assumptions
  - Simple closed population & simple disease
- 3 population categories
  - **Susceptible** ($S$) - people who have not yet been infected
  - **Infected** ($I$) - currently sick and can transmit the disease to **Susceptibles**
  - **Recovered** ($R$) - individuals who have stopped being **Infected**

---

# ODEs

$\large \frac{dS}{dt} = -\frac{\beta}{N} SI$

<!-- The rate of change of the Susceptibles is negative because the number of Susceptibles decreases over time as more people get infected. -->

$\large \frac{dI}{dt} = \frac{\beta}{N} SI - \gamma I$

<!-- Susceptible people become infected, so if the $\beta SI$ term is subtracted from the Susceptible population, $\beta SI$ is added to the Infected population. Then, there are also losses of Infected people when they get recovered; therefore $-\gamma I$ is subtracted. -->

$\large\frac{dR}{dt} = \gamma I$

---

# SIR Dynamics

<img src="https://edu.ella.cx/csb/sir.png" width="80%" />

---

# What happens if we change $\beta$?

<img src="https://edu.ella.cx/csb/sir-with-r.png" width="100%" />

---

# $R_0$ (not to be confused with $R(0)$)

$\Large R_0 = \frac{\beta}{\gamma}$

$R_0 > 1$ describes an outbreak/epidemic.

---

# Limitations and extensions of the classical SIR model

- SEIRS model - latency and temporary immunity (Bjornstad et. al. 2020)
- localized networks
- stochastic effects

---

ohyeah
