# Baja SAE Suspension Development: Analysis & Manufacturing

This repository documents the structural engineering, validation, and manufacturing processes for the suspension A-Arms of a Baja SAE vehicle. The project focuses on bridging the gap between theoretical FEA simulations and real-world physical manufacturing.

##  Project Highlights

### 1. WCS Structural Analysis & Optimization
A comprehensive Worst-Case Scenario (WCS) analysis was conducted to evaluate multi-axis dynamic loads (Bump + Cornering) on the suspension assembly.
* **Material Trade-off Study:** Evaluated the mechanical and elastokinematic behavior of AISI 4130 Chromoly versus 6061-T6 Aluminum.
* **Mass Optimization:** Achieved over 50% unsprung mass reduction across the A-Arm assembly.
* **Validation:** Maintained a Factor of Safety (FOS) > 2.0 against yield strength, utilizing linear static FEA and analyzing specific stiffness metrics.
* **Data Processing:** Implemented Python scripts to automate the post-processing of FEA results, mapping stress distributions along critical paths.

<div align="center">
  <img src="FEA_Results/Screenshot 2026-04-23 184148.png" alt="WCS FEA Simulation" width="700"/>
  <p><i>Figure 1: FEA LowerRear A-Arms Results 1st Configuration.</i></p>
</div>
<div align="center">
  <img src="FEA_Results/Screenshot 2026-04-23 184253.png" alt="WCS FEA Simulation" width="700"/>
  <p><i>Figure 2: FEA LowerRear A-Arms Results 2nd Configuration.</i></p>
</div>
<div align="center">
  <img src="Scripts/Screenshot 2026-04-23 184555.png" alt="WCS FEA Simulation" width="700"/>
  <p><i>Figure 3: Displacement Comparison in LowerRear A-Arms Tubes (Configuration 1 and 2).</i></p>
</div>

### 2. Manufacturing & Steel Fixture Design
To ensure dimensional accuracy and repeatability during the physical build, custom steel welding fixtures were designed and implemented, replacing legacy mdf tooling.
* **Tooling Upgrade & Durability:** Replaced previous MDF fixtures—which degraded and lost tolerance after a maximum of 2 units—with robust steel fixtures capable of producing 15+ A-Arms with minimal dimensional drift.
* **Efficiency Gains:** Slashed manufacturing and welding time by 50% through improved accessibility and modular clamping mechanisms.
* **Hardware Integration:** Successfully manufactured and integrated suspension bushings and control arms for competition standards.

<div align="center">
  <!-- Agrega tu imagen del fixture de acero aquí abajo. Solo cambia el "src" por el nombre de tu archivo (ej. steel_fixture.jpg) -->
  <img src="ruta/a/tu/imagen_fixture.jpg" alt="Steel Fixture and Manufacturing" width="700"/>
  <p><i>Figure 2: Custom steel fixture design and physical manufacturing of the A-Arms.</i></p>
</div>

##  Software & Tools Used
* **CAD Design:** SolidWorks
* **Simulation:** SolidWorks Simulation (FEA)
* **Data Analysis:** Python (Pandas, Matplotlib)
* **Manufacturing:** Technical Drawings, GD&T, Welding, Custom Fixturing

##  Repository Structure
* `/CAD_Models`: Contains the assembly drawings and picture of the geometric models of the A-Arms and the steel fixtures.
* `/FEA_Results`: Contains pictures of the FEA.
* `/Manufacturing`: Contains pictures of the manufacture process.
* `/Scripts`: Contains the results of the post-processing and performance plotting with python (Matplotlib and Pandas).
* `/Documentation`: Engineering reports and FBD calculations.
