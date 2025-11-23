# 🌐 Quantum Computing Portfolio — Hisham Mansour

This repository serves as a **central portfolio** linking my quantum computing projects, hackathon submissions, and algorithm-development work.  
Each project is kept in its original submitted form, and this repository acts as the unified entry point for professional audiences.

---

## 🚀 Highlight Projects

### **1. Quantum Galton Board — Womanium Global Quantum Hackathon 2025**  
🔗 **Repo:** https://github.com/mnshmnsh/Womanium2025--QuantumGaltonBoard  
Implementation of Carney & Varcoe’s [Universal Statistical Simulator](https://arxiv.org/abs/2202.01735), reproducing classical and quantum Galton-board distributions using quantum circuits.

#### 🔧 Key Features
- General algorithm for **n‑level Galton boards** (tested at n=1, 2, and 5).  
- Distributions analyzed: Gaussian (Hadamard gates), Exponential (biased RY rotations), and Hadamard quantum walk (post‑processed symmetry).  
- Simulations performed under four conditions: noiseless baseline, noisy unoptimized, noisy optimized, and noisy optimized with error mitigation.  
- **Statistical validation**: compared simulated vs theoretical distributions using **Total Variation Distance (TVD)** and bin‑by‑bin residual analysis.  
- Circuit diagrams generated for 1‑ and 2‑level boards, showing gate structure and depth.  
- Verified qubit scaling formula \(2n+2\) and depth growth consistent with O(\(n^2\)) construction.

#### 📈 Results
- **Gaussian distributions:**  
  - n=1: Simulated counts matched theory closely (Bin0=4150 vs 4096, Bin1=4042 vs 4096), TVD ≈ 0.013.  
  - n=2: Simulated counts (Bin0=2070, Bin1=4069, Bin2=2053) vs theory (2048, 4096, 2048), TVD ≈ 0.015.  
- **Exponential distributions:**  
  - Bias parameter \(p_{\mathrm{right}} \approx 0.90\).  
  - Noisy runs showed larger deviations, with TVD up to ~0.23–0.33 depending on optimization level.  
- **Hadamard quantum walk (U‑shape):**  
  - Post‑processed symmetry produced distributions with TVD < 0.01 in noiseless runs.  
- **Circuit resources:**  
  - n=1 circuits used 4 qubits, depth ≈ 5.  
  - n=2 circuits used 6 qubits, depth ≈ 14.  
  - Scaling confirmed the \(2n+2\) qubit formula and quadratic depth growth.  
- **Noise analysis:**  
  - FakeSherbrooke backend used to emulate hardware constraints.  
  - Optimization reduced depth by ~20–40% in some cases, though routing sometimes increased gate counts.  
- **Residual plots:**  
  - Highlighted which bins contributed most to distribution differences under noise.
    
---

### **2. Classiq AztecHacks 2024 — Quantum Hackathon**  
🔗 **Repo:** https://github.com/mnshmnsh/Classiq-AztecHacks-2024-Quantum-Hackathon  
Hackathon participation solving all challenge tasks using the Classiq SDK.

#### 🔧 Part A — Challenge Functions
- Implemented all **10 progressively difficult functions** as required:
  - `inplace_square`, `inplace_linear`, `inplace_quadratic`, `inplace_cubic`, `inplace_exponential`
  - `discrete_log_oracle`, `inplace_discrete_logarithm`
  - `equality_oracle`, `inplace_sum`, `sum_of_squares`
- Each function expressed in **reversible arithmetic form** using Classiq’s symbolic quantum number types (`QNum`, `QArray[QBit]`).
- Verified correctness of arithmetic and oracle logic.
- Resource usage (qubits, depth, gate count) reported after synthesis using Classiq’s reporting utilities.

#### 🔧 Part B — Bonus Algorithm
- Implemented the **W₃ Werner state**:
  - Superposition of `001`, `010`, `100`.
  - Constructed via a sequence of RY, X, CH, and CX gates.
  - Demonstrates entanglement structure generation and state preparation.
- Synthesized and executed with Classiq, confirming correct distribution of measurement outcomes.

#### 📈 Results
- All 10 challenge functions implemented and tested successfully.  
- Bonus Werner state prepared and validated.  
- Resource reporting provided for synthesized circuits, highlighting qubit usage and gate counts.

---

### **3. Quantum Utility & Error Mitigation — 2D Ising Model**  
🔗 **Repo:** https://github.com/mnshmnsh/Development-of-Novel-Quantum-Algorithms  
QAOA and Trotterized 2D Ising simulation with artificial noise injection. Ground-state energy recovered via Zero-Noise Extrapolation (ZNE), guided by [Kim et al., Nature 615, 596–600 (2023)](https://doi.org/10.1038/s41586-023-06096-3).

#### 🔧 Key Features
- QAOA applied to the **2D transverse‑field Ising model**.  
- Trotterized time evolution via Suzuki product formula.  
- Artificial noise layers added to study degradation.  
- **Zero Noise Extrapolation (ZNE)** applied to recover ground‑state energy.  
- Energy vs noise level plots demonstrating extrapolation improvement.  

#### 📈 Results
- Plots show noisy vs extrapolated energies, confirming ZNE effectiveness.  
- Demonstrated meaningful results despite hardware noise.  

---

## 🧠 Skills & Tools

### **Quantum**
Qiskit • Classiq SDK • Pennylane • D‑Wave Ocean SDK
Tensor Networks • QAOA • VQE • Amplitude encoding
Variational circuits • Quantum walks • Quantum simulation 
ZNE • PDE solvers  

### **Classical / ML**
Python • PyTorch • NumPy • SciPy • Data visualization  

---

## 📫 Contact

**LinkedIn:** https://www.linkedin.com/in/hisham-mansour-554237281  
**GitHub:** https://github.com/mnshmnsh  
