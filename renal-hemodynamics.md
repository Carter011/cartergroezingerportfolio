[Home](index.md) | [Projects](projects.md) | [About](about.md) | [Resume](resume.pdf)

---
title: Renal Artery Hemodynamics
---

# Renal Artery Hemodynamics Using the Lattice Boltzmann Method

## Project Overview
This project investigated how renal artery branch stent geometry influences local blood flow following fenestrated endovascular aneurysm repair (F/B EVAR). Using Lattice Boltzmann–based computational modeling, I analyzed how geometric factors such as branch angle affect flow separation, recirculation, and residence time near the renal artery ostium.

The work was conducted in the Multiscale Advection Diffusion Analysis Laboratory (MADAL) at Embry-Riddle Aeronautical University and was submitted for presentation at the ASME Fluids Engineering Division Summer Meeting (FEDSM 2026).

---

## Engineering Motivation
Renal artery occlusion is a known complication following complex endovascular aneurysm repair procedures. While modern stent designs allow preservation of renal perfusion, subtle changes in branch geometry can significantly alter local hemodynamics.

Clinical imaging provides strong anatomical detail but limited insight into flow behavior such as recirculation and shear stress distribution. Computational modeling enables detailed interrogation of these flow features, helping explain mechanisms that may contribute to thrombosis and vessel occlusion.

This project focused on understanding how branch stent angle influences flow behavior at the renal artery entrance.

---

## Modeling Approach
- Constructed a **patient-generic vascular geometry** representing an aortic segment with a renal branch stent  
- Simulated steady-state flow using a **GPU-accelerated Lattice Boltzmann Method (LBM)**  
- Applied pressure-driven inlet and outlet boundary conditions  
- Enforced no-slip conditions at vessel walls  
- Post-processed results using velocity contours, vector fields, and streamlines  

LBM was selected for its ability to efficiently resolve flow separation and recirculation while maintaining numerical stability in complex geometries.

---

## Key Flow Features Observed
Across all simulations, several consistent hemodynamic features were observed:

- Formation of **recirculation zones** near the renal artery ostium  
- Presence of **low-velocity regions** adjacent to the downstream branch wall  
- Strong sensitivity of flow separation to **branch stent tilt angle**  

As branch angle decreased, recirculation regions expanded and particle residence time near the branch entrance increased—conditions commonly associated with elevated thrombogenic risk.

---

## Validation and Comparison
Computed flow fields were compared qualitatively against previously published computational studies. Key features such as recirculation location, velocity redistribution, and branch flow partitioning showed strong agreement with reference results.

This agreement supports the suitability of LBM-based solvers for investigating post-operative renal artery hemodynamics and complex vascular flow environments.

---

## Visual Results

![Renal artery velocity field and recirculation zones](assets/renal-hemodynamics/flow-fields.png)

*Velocity magnitude and streamline visualizations highlighting recirculation near the renal artery ostium.*

![Effect of branch angle on renal artery flow](assets/renal-hemodynamics/branch-angle.png)

*Region of interest illustrating increased flow separation.*

---

## Outcomes and Takeaways
- Demonstrated the influence of branch stent geometry on renal artery hemodynamics  
- Identified flow features associated with thrombotic risk and branch occlusion  
- Validated the use of LBM for high-fidelity vascular flow modeling  
- Provided computational insight that may inform stent design and deployment strategies  

---

## Publication
This work was submitted to and accepted for presentation at the ASME Fluids Engineering Division Summer Meeting (FEDSM 2026).

**Groezinger, C., Das, A., Chen, L.**  
*An In-Silico Investigation of Renal Artery Hemodynamics in Fenestrated Endovascular Aneurysm Repair Using the Lattice Boltzmann Method*  
ASME FEDSM 2026.

📄 **[View full publication (PDF)](assets/renal-hemodynamics/FEDSM_184313.pdf)**
