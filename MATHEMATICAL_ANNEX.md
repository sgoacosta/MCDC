# Mathematical Annex – MCDC 2.0
This document summarizes the **geometric** and mathematical formalization of the Double Celestial Cones Model (MCDC 2.0) for technical review by the community.

## Purpose of this annex
- Present the equations and assumptions of the model.
- Provide traceability of the mathematical decisions made.
- Enable critical evaluation without overloading the main README.

## 1. Basic geometry of MCDC 2.0
- Two fixed cones: Polar Cone (north celestial pole) and Crucial Cone (south celestial pole).
- Dynamic Equatorial Belt (CED): dynamic east–zenith–west arc that represents the apparent motion of the sky.
- Observer‑centric approach: the origin of the system is the observer on the Earth’s surface.

### 1.1 Cones in spherical coordinates
- Spherical coordinates \((r, \theta, \varphi)\) with:
  - \(\theta\): polar angle (celestial latitude).
  - \(\varphi\): azimuth angle (celestial longitude).
- Idealized cone:
  - \(\theta = \theta_0\) defines the cone opening.
- Special cases:
  - Polar Cone: \(\theta = \theta_{\text{north}}\).
  - Crucial Cone: \(\theta = \theta_{\text{south}}\).

### 1.2 Cones in classical conical form
In cylindrical or Cartesian coordinates a cone can be written as:
- \(r = h \tan(\alpha)\), where:
  - \(h\): height from the vertex (celestial pole).
  - \(\alpha\): opening angle.
  - \(r\): radius of the section at height \(h\).

## 2. Dynamic Equatorial Belt (CED)
The CED is modeled as an arc on a sphere of radius \(R\).

### 2.1 Temporal parametrization
- Angular position:
  \[
  \varphi(t) = \omega t + \varphi_0
  \]
  where:
  - \(\omega\): angular velocity of rotation (≈ \(2\pi / 23.934\,\text{h}\)).
  - \(\varphi_0\): initial phase (position at \(t = 0\)).

- Planar representation:
  \[
  x(t) = R \cos(\omega t + \varphi_0), \quad
  y(t) = R \sin(\omega t + \varphi_0)
  \]

### 2.2 CED layers
The model admits concentric layers:
- Inner layer: Sun, Moon and planets.
- Middle layer: zodiac constellations or other relevant bands.
- Outer layer: stellar background.

## 3. Precession of the poles
To reflect that the celestial poles are not strictly fixed:

### 3.1 Precession of Earth’s axis
- Mean precession rate: ≈ \(50.29''\) per year.
- Simplified angular model:
  \[
  \theta(t) = \theta_0 + k\,t
  \]
  where \(k\) encodes the precession rate in radians per year.

### 3.2 From Polaris to Vega (example)
- In the north:
  - Today: cone vertex near Polaris.
  - In ~12.000 years: vertex near Vega.
- In the model:
  - The vertex of the Polar Cone traces a circle (or closed trajectory) on the celestial sphere over the precession cycle.
  - This trajectory can be parametrized in equatorial or ecliptic coordinates as a closed curve with a period of ≈ 25.772 years.

## 4. Generalization to other bodies
The MCDC scheme is not limited to Earth:

- Any rotating body:
  - Cones anchored to its rotation poles.
  - CED adapted to its equatorial plane and rotation period.
- This allows:
  - Defining “sky” analogues for planets, stars, or fictional systems.
  - Exploring differences in axis tilt, periods and precession.

## 5. Scope and limitations of the model
- Scope:
  - Intuitive geometric model for teaching and visualization.
  - Basis for more precise formalizations using modern numerical data.
- Limitations:
  - Does not yet include all high‑precision astronomical effects (aberration, nutation, relativity, etc.).
  - Accuracy depends on how current ephemerides and catalogs are integrated.

## 6. Notes for reviewers
- This annex is intended as a technical support document.
- Feedback on:
  - Internal consistency of the equations.
  - Possible extensions (nutation, aberration, IAU models).
  - Numerical implementations and comparisons with astronomical software,
  is welcome via issues or additional documentation.
