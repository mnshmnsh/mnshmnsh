# 🌐 Quantum Computing Portfolio — Hisham Mansour

This repository serves as a **central portfolio** linking my quantum computing projects, hackathon submissions, and algorithm-development work.  
Each project is kept in its original submitted form, and this repository acts as the unified entry point for professional audiences.

---

## 🚀 Highlight Projects

### **1. Quantum Galton Board — Womanium Global Quantum Hackathon 2025**  
🔗 **Repo:** https://github.com/mnshmnsh/Womanium2025--QuantumGaltonBoard  
Implementation of Carney & Varcoe’s [Universal Statistical Simulator](https://arxiv.org/abs/2202.01735), reproducing classical and quantum Galton-board distributions using quantum circuits.

#### 🔧 Key Features
- General algorithm for **n‑level Galton boards** (scalable circuit construction).  
- Distributions tested: Gaussian, Exponential, Hadamard quantum walk.  
- Noise modeling and correlated readout error mitigation (`qiskit_experiments`).  
- Statistical validation using **Total Variation Distance (TVD)** and residual analysis.  
- Circuit diagrams generated for n=1, 2, 5 levels.  
- Demonstrated **O(n²)** quantum resource scaling vs classical O(2ⁿ).  

#### 📈 Results
- Verified Gaussian, Exponential, and Hadamard distributions against theory.  
- Strong agreement achieved (TVD < 0.1 in optimized runs).  
- Residual plots highlight systematic vs random errors.  

---

### **2. Classiq AztecHacks 2024 — Quantum Hackathon**  
🔗 **Repo:** https://github.com/mnshmnsh/Classiq-AztecHacks-2024-Quantum-Hackathon  
Hackathon participation solving all challenge tasks using the Classiq SDK.

#### 🔧 Key Features
- Arithmetic functions implemented directly in Classiq SDK.  
- **W₃ Werner state**: superposition of `001`, `010`, `100` via decomposed Toffoli (CNOT sequence).  
- Pipeline from high‑level model → synthesized circuits → resource reporting (qubits, depth, gate count).  
- Bonus: custom weighted‑sum circuit with entanglement structure generation.  
- Progressive difficulty: each function builds on prior concepts.  

#### 📈 Results
- Verified correctness of all 10 functions.  
- Resource usage reported for each synthesized circuit.  
- Bonus algorithm implemented with entanglement‑based arithmetic.  

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

**LinkedIn:** [https://www.linkedin.com/in/hisham-mansour-554237281]  
**GitHub:** https://github.com/mnshmnsh  
