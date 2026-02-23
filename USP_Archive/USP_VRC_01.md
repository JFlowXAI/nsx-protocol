# USP Variable Roles Contract (v0.1)

## Purpose

This document defines the **non-overlapping functional roles** of core USP dynamic variables.
Its purpose is to prevent parameter redundancy and ensure mathematical clarity
before experimental expansion.

The guiding principle:

> Each variable must control ONE distinct aspect of the system.

---

# 1. System Overview

USP models experiential selection as a receiver/transducer-mediated projection
from a potentiality spectrum.

Outcome probability:

\[
p(i,t)=\left|\langle \Phi_i(R,t) \mid \Psi_S \rangle\right|^2
\]

Receiver state depends on dynamic parameters governing availability,
alignment, and identity structure.

---

# 2. Variable Definitions

## 2.1 Belief Bandwidth — \( \beta(t) \)

### Role
Controls **spectral availability**.

Defines how much of the possibility spectrum can participate in selection.

### Interpretation
- Large \( \beta \): wide accessible outcome space
- Small \( \beta \): restricted outcome availability

### Dynamics

\[
\frac{d\beta}{dt}
=
-\gamma(\beta-\beta_0(t))+\eta(t)
\]

Where:

- \( \gamma \) = identity elasticity
- \( \beta_0(t) \) = drifting baseline
- \( \eta(t) \) = environmental/somatic noise

### Governs
Amplitude envelope only.

NOT interference.

---

## 2.2 Coherence — \( C(t) \)

### Role
Controls **interference sensitivity**.

Determines whether components combine constructively or destructively.

### Interpretation
- \(C=1\): coherent regime (interference active)
- \(C=0\): classical mixture (no interference)

### Dynamics

\[
\frac{dC}{dt}
=
\alpha A(t)(1-C)-\lambda\eta(t)C
\]

Where:

- \(A(t)\) = alignment/resonance signal
- \(\eta(t)\) = noise
- \(\alpha,\lambda\) = growth/decay constants

### Governs
Phase interaction only.

NOT spectral width.

---

## 2.3 Effective Bandwidth

To avoid redundancy:

\[
\beta_{\text{eff}}(t)=C(t)\cdot\beta(t)
\]

Meaning:

- belief determines availability
- coherence determines usability

---

## 2.4 Phase Response — \( \phi_R(x,t) \)

### Role
Defines relative phase alignment between receiver and spectrum modes.

Receiver mode:

\[
|\Phi_i(R,t)\rangle
=
e^{i\phi_R(x,t)}
F(\beta(t),\iota(t),\mathcal{I}(t))
\]

### Operational Status
Phase is **not directly measurable**.

It is inferred through coherence proxies.

---

## 2.5 Intention — \( \iota(t) \)

### Role
Defines directional displacement within accessible spectrum.

Penalty structure:

\[
\exp\left(
-\frac{\iota(t)^2}{2(\sigma_S^2+\beta(t)^2)}
\right)
\]

Intention without bandwidth produces negligible effect.

---

# 3. Orthogonality Principle

Variables must remain independent:

| Variable | Controls |
|---|---|
| \( \beta(t) \) | Availability (amplitude width) |
| \( C(t) \) | Interference sensitivity |
| \( \phi_R \) | Relative phase alignment |
| \( \iota(t) \) | Directional targeting |

No variable duplicates another’s function.

---

# 4. Timescale Separation

System stability requires:

- Fast variable: \(C(t)\) (minutes–hours)
- Slow variable: \(\beta(t)\) (hours–days)

This prevents dynamical degeneracy.

---

# 5. Ambivalence Definition

Ambivalence occurs when:

\[
\beta(t)\ \text{high}
\quad \text{and} \quad
2\operatorname{Re}(\psi_1^*\psi_2) < 0
\]

High availability + destructive interference.

Result:
Energy without behavioral motion.

---

# 6. Design Rule

Before adding new parameters:

> Ask: What system property does this uniquely control?

If answer duplicates an existing variable → reject parameter.

---

**Status:** Structural stabilization document
**Purpose:** Pre-experimental refinement