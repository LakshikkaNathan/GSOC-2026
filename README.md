# GSoC 2026 — QMLHEP6

**ML4Sci | Learning quantum representations of classical high energy physics data with contrastive learning**

Lakshikka Sithamparanathan | Cleveland State University

---

## Prerequisite Tasks

| Notebook | Task |
|---|---|
| `Task_I_Quantum_Circuits.ipynb` | Quantum circuits + SWAP test (PennyLane) |
| `Task_II_Classical_GNN.ipynb` | GCN & GAT for quark/gluon jet classification |
| `Task_III_Open_Task.ipynb` | Commentary on quantum machine learning |
| `Task_VI_Quantum_Contrastive_Learning.ipynb` | Quantum contrastive learning with SWAP test fidelity |

## Key Results

**Task II** (50k jets, k-NN graph k=8)

| Model | Accuracy | AUC |
|---|---|---|
| GCN (3-layer) | 0.784 | 0.856 |
| GAT (3-layer, 4 heads) | 0.717 | 0.830 |

**Task VI** (MNIST, 8 qubits, 17 total wires)

| Metric | Result |
|---|---|
| Same-class fidelity | 0.8158 ± 0.1401 |
| Different-class fidelity | 0.6292 ± 0.1516 |
| Fidelity gap | 0.1866 |
| Classification accuracy | 77.0% @ threshold 0.667 |

## Setup

```bash
pip install pennylane torch torchvision torch-geometric
```
