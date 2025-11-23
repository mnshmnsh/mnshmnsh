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
  - n=1: Simulated counts Bin0=4150 vs theory 4096, Bin1=4042 vs theory 4096 → TVD ≈ 0.013.  
  - n=2: Simulated counts Bin0=2070, Bin1=4069, Bin2=2053 vs theory (2048, 4096, 2048) → TVD ≈ 0.015.  
- **Exponential distributions:**  
  - Bias parameter \(p_{\mathrm{right}} \approx 0.90\).  
  - Noisy runs showed larger deviations, with TVD up to ~0.23–0.33 depending on optimization level.  
- **Hadamard quantum walk (U‑shape):**  
  - Post‑processed symmetry produced distributions with TVD < 0.01 in noiseless runs.  
- **Circuit resources:**  
  - n=1 circuits: 4 qubits, depth ≈ 5.  
  - n=2 circuits: 6 qubits, depth ≈ 14.  
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
- Implemented all **10 progressively difficult functions**:
  - `inplace_square`, `inplace_linear`, `inplace_quadratic`, `inplace_cubic`, `inplace_exponential`
  - `discrete_log_oracle`, `inplace_discrete_logarithm`
  - `equality_oracle`, `inplace_sum`, `sum_of_squares`
- Each function expressed in **reversible arithmetic form** using Classiq’s symbolic quantum number types (`QNum`, `QArray[QBit]`).  
- Verified correctness of arithmetic and oracle logic.  
- **Resource reporting after synthesis:**  
  - Example: `inplace_quadratic` synthesized with depth ≈ 12, gate count ≈ 40.  
  - `inplace_discrete_logarithm` synthesized with depth ≈ 60+, gate count ≈ 200+.  
  - These values confirmed the circuits scale with function complexity.

#### 🔧 Part B — Bonus Algorithm
- Implemented the **W₃ Werner state**:
  - Superposition of `001`, `010`, `100`.  
  - Constructed via a sequence of RY, X, CH, and CX gates.  
  - Synthesized circuit used 3 qubits, depth ≈ 12, with ~8 CX gates.  
- Executed with Classiq simulator, producing measurement outcomes distributed across the three target states.

#### 📈 Results
- All 10 challenge functions implemented and tested successfully.  
- Resource usage (qubits, depth, gate counts) reported for each synthesized circuit.  
- Bonus Werner state prepared and validated, with measurement counts confirming the expected superposition.

---

### **3. Quantum Utility & Error Mitigation — 2D Ising Model**  
🔗 **Repo:** https://github.com/mnshmnsh/Development-of-Novel-Quantum-Algorithms  
QAOA and Trotterized 2D Ising simulation with artificial noise injection, guided by [Kim et al., Nature 615, 596–600 (2023)](https://doi.org/10.1038/s41586-023-06096-3).

#### 🔧 Key Features
- 2D Ising Hamiltonian (4×4 lattice, periodic boundary conditions) encoded with Pyomo.  
- QAOA with 5 layers, 100 iterations, CVaR parameter \(\alpha=0.7\).  
- Suzuki–Trotter decomposition for Hamiltonian evolution.  
- Circuit synthesized under depth and width constraints.  
- Random noise added to Pauli coefficients; Zero‑Noise Extrapolation (ZNE) applied via linear fit.

#### 📈 Results
- Circuit width = 16 qubits, depth ≈ 91.  
- Gate composition: 320 CX, 240 RZ, 80 RX, 16 H.  
- Best solution cost ≈ –960 with probability ≈ 0.71.  
- Energy convergence observed after ~80 iterations.  
- Noiseless energy ≈ –699.7; extrapolated energy via ZNE ≈ –670.6.  
- ZNE produced extrapolated energies close to the noiseless baseline, demonstrating mitigation of noise effects.

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

  
