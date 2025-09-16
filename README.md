# ELATHA-Lunar-Sample-Collection-Mission
ELATHA Lunar sample collection mission CAD and modelling portfolio.

# MMME4105 Lunar Rover Sample Collection Mission - CAD Modelling Portfolio

> Academic group design project demonstrating CAD modelling of a three-element lunar mission: **Orbiter**, **Lander-Ascender**, and **Rover**. Focus on a model-up, first-principles approach, robust assemblies, parameters, and kinematics to show design intent and handover readiness.
> Credit to group members: Christian McMahon-Walsh, Oliver Legon, Luca Mendes, Max Williams, Alexander Rose

---

## Contents

- [Project scope](#project-scope)
- [Repo contents](#repo-contents)
- [Assemblies and mechanisms overview](#assemblies-and-mechanisms-overview)
  - [Orbiter](#orbiter)
  - [Lander-Ascender](#lander-ascender)
  - [Rover](#rover)
- [How to use these materials](#how-to-use-these-materials)
- [What this showcases](#what-this-showcases)
- [Licence and attribution](#licence-and-attribution)

---

## Project scope

- Mission elements: **Orbiter**, **Lander-Ascender**, **Rover**, with kinematic sample transfer.
- Approach: bottom-up modelling, design from first principles, early parameterisation of interfaces and envelopes.
- Evidence provided here: **presentation deck** and **silent walkthrough video** highlighting modelling techniques, assemblies, and motion studies.

---

## Repo contents


- **Presentation (PPTX):** slides with model trees, projections, subsystem layouts, and mechanism snapshots.  
  [Open the presentation](assets/MMME4105%20Group%201%20-%20Modelling%20Portfolio%20%28No%20Sound%29.pptx)

- **Walkthrough video (MP4):** silent screen capture of key modelling techniques, assemblies, and kinematic reviews.  
  [Watch the video](assets/MMME4105%20Group%201%20-%20Modelling%20Portfolio.mp4)

> Note: CAD source files are not included in this repository.

---

## Assemblies and mechanisms overview

### Orbiter

- **Structure:** internal components sized the primary frame; shelves and walls created to support mounting. Pads, pockets, and mirroring used to exploit symmetry.
- **Subsystem placement:** reaction wheels, cold gas tank and thrusters, EPS, battery, radiator, sun sensors, star tracker, horizon sensor, transceiver, MLI, solar panel, antenna pointing system. Equipment arranged about the centre of gravity.
- **Antenna pointing:** bi-axial gimbal with motion limits and collision-free clearances. Antenna and pointing mechanism separated into subassemblies for independent motion review.

### Lander-Ascender

- **Structure and interfaces:** interface plates built with pads and ribbing; fillets suggest welded joints. Components positioned by defined interfaces.
- **Subsystems:** landing gear, rover ramp, RCS thrusters, bi-propellant main engine, propellant and pressurant tanks, pipelines, battery, solar panels, antenna, RTG, sample storage, cameras, MLI.
- **Mechanisms:**
  - **Landing gear:** four replicated leg sets with upper suspension assemblies, control arms, and landing legs imported as separate parts to allow movement at top level.
  - **Rover ramp and docking:** deployment kinematics for ramp; docking and undocking sequence for the ascender.
- **Sample transfer alignment:** placeholder docking ports on rover and ascender aid alignment during transfer.

### Rover

- **Structure:** bottom-up assembly. Chassis and sample collection system sized around components to minimise profile.
- **Subsystems:** OBC, EPS (battery, BCR), TT&C transceiver, motor controller, accelerometer, RTG, NAVCAM and HAZCAMs, floodlights, rocker-bogie, tether housing, sample storage with carousel. Drawings presented as third-angle projections in the deck.
- **NAVCAM mechanism:** camera, housing, and mast fixed with two revolute joints providing bi-axial rotation.
- **Sample Collection System (SCS):**
  - **Arms:** parameterised for 2-DoF planar collection and deposit to front or rear containers.
  - **Sampler:** scoop sized for fill rate; air pump flush for dust control; funnelled guidance; three servos actuate a seal via a central seal rod for redundancy.
  - **Storage:** six containers on a sample carousel with a seal carousel and a compact press. Motion driven from a single revolute on the seal carousel motor; seals retained with cylindrical constraints after contact constraints proved unreliable.
  - **Transfer:** carousel lowers by tethers after hold-down release; guiding geometry ensures reliable handover with small belly clearance.

---

## How to use these materials

1. **Skim the presentation** to understand scope, naming, and subsystem breakdown.
2. **Watch the walkthrough video** to see assemblies and mechanisms in motion, with attention to:
   - Parameter-driven interfaces and envelope updates
   - Separation of mechanisms for independent kinematic checks
   - Clearance and range-of-motion validation across mission phases

---

## What this showcases

- **Configuration management:** consistent naming, structured breakdown, and separation of mechanisms for reuse and clarity.
- **Parametric design intent:** interfaces and critical envelopes driven by parameters to enable rapid iteration with minimal rebuild issues.
- **Mechanism fidelity:** engineering connections reflect realistic motion limits and allow early collision checks.
- **First-principles design:** structures sized from subsystem budgets and physical constraints, not legacy geometry.
- **Realism:** off-the-shelf components modelled where useful to anchor interfaces and volumes.

---

## Licence and attribution

- **Licence:** see `LICENCE` in this repository.
- **Attribution:** MMME4105 Group 1 - Aerospace Group Design Project. CAD models, drawings, and media as listed above.


All rights reserved.

No part of this project, including CAD models, documentation, video, or presentation materials,
may be copied, modified, distributed, or used for commercial or academic purposes
without prior written permission from the authors.
