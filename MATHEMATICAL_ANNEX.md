# Mathematical Annex – MCDC 2.0
The MCDC 2.0 model is introduced in the main README as an intuitive geometric representation of the observable sky. This annex focuses exclusively on its mathematical structure.

## Purpose of this annex
- Present the equations and assumptions of the model.
- Provide traceability of the mathematical decisions made.
- Enable critical evaluation without overloading the main README.

## 1. Basic geometry of MCDC 2.0
- Two fixed cones: Polar Cone (north) and Crucial Cone (south).
- CED (Cincture Equatorial Dynamic): join of the cones dynamic east–zenith–west arc that represents the apparent motion of the sky. 
- Observer‑centric approach: in this case the origin of the system is the observer on the Earth’s surface.

### 1.1 Cones in classical conical form
In cylindrical or Cartesian coordinates a cone can be written as:
- $r$ = $h$ tan(α), where:
  - $h$: height from the vertex (celestial pole).
  - α: opening angle.
  - $r$: radius of the section at height $h$.

### 2. Diameter of the CED

The CED defines the observable limit of the sky in the east–west direction. Its angular extent is fixed by the celestial equator, but its physical scale is determined by the most distant objects visible at the extremes.

Let $d_{\text{max}}$ be the maximum observable distance toward the east (or west). Then the diameter of the CED is:

$D_{\text{CED}} = 2 \cdot d_{\text{max}}$

This value represents the maximum separation between two observable points in opposite directions along the celestial equator.

In the context of the MCDC, $d_{\text{max}}$ corresponds to the distance of the farthest star or galaxy detectable near the eastern and western horizons. The CED diameter becomes a fundamental geometric parameter of the observable universe.

From this, other quantities can be derived, such as:

- The **radius of the observable universe** $R_u \approx d_{\text{max}}$.
- The **volume** of the observable region.
- The **scale** for computational limits (as used in the P vs NP argument).

## 3. Precession of the poles
To reflect that the celestial poles are not strictly fixed:

### 3.1 Precession of Earth’s axis
- Mean precession rate: ≈ 50.29'' per year.
- Simplified angular model: θ(t) = θ₀ + k t
   where \(k\) encodes the precession rate in radians per year.

### 3.2 From Polaris to Vega (example)
- In the north:
  - Today: cone vertex near Polaris.
  - In ~12,000 years: vertex near Vega.
- In the model:
  - The vertex of the Polar Cone traces a circle (or closed trajectory) on the celestial sphere over the precession cycle.
  - This trajectory can be parametrized in equatorial or ecliptic coordinates as a closed curve with a period of ≈ 25,772 years.

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
