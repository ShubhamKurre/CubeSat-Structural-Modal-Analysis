# 🛰️ Structural and Modal Analysis of a CubeSat Satellite Frame

This project involves the **static, modal, pre-stressed, and buckling analysis** of a 1U CubeSat satellite frame to evaluate its structural integrity and dynamic behavior under launch and orbital conditions.  
The objective was to ensure that the CubeSat frame is lightweight, rigid, and free from resonance within the expected launch frequency range.

---

## 🎯 Objectives
- Evaluate the **mechanical strength** and **stiffness** of a CubeSat structure.
- Determine the **natural frequencies** and **mode shapes** to ensure resonance safety.
- Analyze **buckling stability** under compressive launch loads.
- Compare different **aluminum alloys** for optimal strength-to-weight performance.

---

## 🧰 Tools & Software
- **ANSYS Workbench (Mechanical Module)** – Structural, Modal, and Buckling Analyses  
- **SolidWorks / Fusion 360** – CAD modeling of CubeSat frame  
- **MS Excel / MATLAB** – Data processing and visualization  

---

## ⚙️ Methodology

### 1. Geometry & Meshing
- 1U CubeSat frame (100 mm × 100 mm × 100 mm) with internal brackets and mounting points.
- Fine tetrahedral mesh with element size 2–3 mm for convergence accuracy.

### 2. Static Structural Analysis
- Launch loads applied as equivalent acceleration and constraints on mounting faces.
- **Results:**  
  - Maximum deformation: **0.42 mm**  
  - Maximum von Mises stress: **35 MPa**  
  - Safety factor > 2 for all alloys.

### 3. Modal Analysis
- Boundary-free condition to obtain natural frequencies and mode shapes.  
- **First three natural frequencies:**  
  | Mode | Frequency (Hz) | Mode Description          |
  |------|----------------|----------------------------|
  | 1    | 320 Hz         | Bending (longitudinal)     |
  | 2    | 450 Hz         | Torsional (diagonal twist) |
  | 3    | 610 Hz         | Bending (transverse)       |

  Since launch vibration spectra are typically < 200 Hz, **resonance is avoided.**

### 4. Pre-Stressed & Buckling Analysis
- Included pre-loads from fasteners and compressive stresses.
- **Buckling factor:** > 1.8 → structurally stable under launch compression.

### 5. Material Comparison
| Material | Yield Strength (MPa) | Density (g/cm³) | Remarks |
|-----------|----------------------|-----------------|----------|
| Al 5052-H32 | 193 | 2.68 | Ductile, corrosion resistant |
| Al 6061-T6 | 276 | 2.70 | Balanced, cost-effective |
| Al 7075-T6 | 503 | 2.81 | High strength, aerospace-grade ✅ |

**Selected:** *Al 7075-T6* for superior stiffness-to-weight ratio.

---

## 📊 Key Results

| Parameter | Value | Comment |
|------------|--------|----------|
| Max Deformation | 0.42 mm | Acceptable rigidity |
| Max Stress | 35 MPa | Below yield for all alloys |
| Buckling Factor | > 1.8 | Safe under launch loads |
| 1st Mode Frequency | 320 Hz | Resonance-free region |

---

## 📈 Visualization

**Static Deformation (mm)**  
![Deformation Plot](Results/deformation_mode1.png)

**Stress Distribution (von Mises, MPa)**  
![Stress Plot](Results/stress_contours.png)

**Mode Shapes**  
![Mode Shapes](Results/mode_shapes.png)

---

## 📚 Learning Outcomes
- Developed expertise in **finite element analysis (FEA)** using ANSYS.
- Understood **modal and buckling stability criteria** for aerospace structures.
- Learned to interpret **resonance and vibration safety** in satellite design.
- Practiced **material selection and optimization** for lightweight frames.

---

## 🧭 Future Scope
- Integrate **thermal-structural coupling** to simulate orbital heating.
- Extend to **multi-U CubeSat** configurations with deployable mechanisms.
- Validate simulation with **vibration table experiments**.

---

## 👨‍💻 Author
**Shubham Kurre**  
Mechanical Engineering | Thermal & Structural Systems | MATLAB | ANSYS  
[LinkedIn](https://linkedin.com/in/) • [GitHub](https://github.com/shubhamkurre)

---

### 📂 Repository Structure
