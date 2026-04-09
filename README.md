# ⚛️ Quantum Tunnelling Simulation

An interactive, browser-based simulation for visualising quantum tunnelling — the phenomenon where a particle crosses a classically forbidden energy barrier due to the wave nature of matter.

Built as part of the Applied Physics curriculum at **NMIMS MPSTME**, Semester 2.

---

## 🖥️ Live Preview

> Open `quantum_tunnelling.html` directly in any modern browser — no server, no install, no dependencies.

---

## ✨ Features

- **Four simulation modes** — Approximate, Exact (sinh/sin), Barrier, and Potential Well
- **Real-time wavefunction plot** — Visualises Ψ(x) and the potential barrier V(x) simultaneously using Chart.js
- **Transmission vs Barrier Width graph** — Compare Approximate vs Exact model curves dynamically
- **3D particle visualisation** — Live Three.js render of a particle approaching and tunnelling through a barrier
- **Transmission Probability calculator** — Updates in real-time as you adjust energy, barrier height, and width
- **Physics Reference panel** — Inline explanations of the underlying quantum mechanics (Heisenberg's uncertainty principle, de Broglie wavelength, evanescent wavefunction decay)
- **Formula display** — LaTeX-style inline equations for both Approximate and Exact transmission formulas

---

## 🧪 Physics Behind It

Quantum tunnelling occurs when a particle's total energy **E < V₀** (below the barrier potential), yet the wavefunction decays exponentially *through* the barrier rather than dropping to zero — giving a non-zero probability of the particle appearing on the other side.

**Approximate formula (thick barrier approximation, κL >> 1):**

```
T ≈ 16(E/V₀)(1 - E/V₀) · e^(-2κL)
```

**Exact formula (all regimes):**

```
T = [1 + (V₀² · sinh²(κL)) / (4E(V₀ - E))]⁻¹
```

Where `κ = sqrt(2m(V₀ - E)) / ℏ` is the decay constant inside the barrier.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Structure & Logic | HTML5, Vanilla JavaScript |
| Styling | CSS3 (custom design system, no frameworks) |
| 2D Charts | [Chart.js 4.4.1](https://www.chartjs.org/) |
| 3D Rendering | [Three.js r128](https://threejs.org/) + OrbitControls |
| Fonts | JetBrains Mono, Inter (Google Fonts) |

---

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/eashankgiriTL/Quantum_Tunnelling_Simulation.git

# Navigate into the folder
cd Quantum_Tunnelling_Simulation

# Open in browser
open quantum_tunnelling.html   # macOS
# or just double-click the file on Windows/Linux
```

No npm. No build step. No server required.

---

## 📁 File Structure

```
Quantum-Tunnelling-Simulation/
│
├── quantum_tunnelling.html     # Complete simulation (self-contained)
└── README.md
```
---

## 👤 Author

**Eashan K Giri**
MBA Tech (Computer Engineering) — NMIMS MPSTME, Mumbai (2025–30)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-eashankgiri108-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/eashankgiri108/)
[![GitHub](https://img.shields.io/badge/GitHub-eashankgiriTL-black?style=flat&logo=github)](https://github.com/eashankgiriTL)

---

## 📄 License

This project is open for academic and educational use.
