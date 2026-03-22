**Dineth Jayakody**  
**Course:** CS 800 – Research Methods  
**Assignment:** 5  

---

# Deep Tissue Imaging: From DEEP to DEEP-squared

## Assignment description

This folder contains materials for **CS 800 – Research Methods (Assignment 5)**. The assignment focuses on analyzing and presenting a **pair of related research papers** and clearly explaining the **relationship between them**.

The selected papers are:

1. **DEEP (2021)** – Introduces a computational imaging method for de-scattering in wide-field two-photon microscopy.
2. **DEEP-squared (2023)** – Extends DEEP using deep learning to significantly improve reconstruction speed and efficiency.

The presentation covers:

- Fundamentals of **two-photon microscopy**
- The **DEEP framework** (physics + optimization)
- The **DEEP-squared framework** (physics + deep learning)
- A detailed explanation of **how DEEPsquared builds upon DEEP**

---

## Repository structure

```
.
├── README.md
└── papers/
    ├── DEEP_paper.pdf
    └── DEEP-squared_paper.pdf
```

- **`papers/`** – Contains the two research papers used for this assignment:
  - DEEP paper (*Science Advances*, 2021)
  - DEEP-squared paper (*Light: Science & Applications*, 2023)

---

## Papers

### 1. DEEP (Paper 1)

**Title:** De-scattering with Excitation Patterning enables rapid wide-field imaging through scattering media  
**Authors:** Zheng et al.  
**Venue:** *Science Advances*, 2021  

### 2. DEEP-squared (Paper 2)

**Title:** DEEP-squared: Deep Learning Powered De-scattering with Excitation Patterning  
**Authors:** Wijethilake et al.  
**Venue:** *Light: Science & Applications*, 2023  

---

## Google Slides presentation

[Dineth Jayakody – Assignment 5 – Presentation](https://docs.google.com/presentation/d/1_GUbJwxwzkbMCUXtQrnvmJCXjfX3Srq9B1J2aeImJqE/edit?usp=sharing)

---

## BibTeX entries

### DEEP (2021)

```bibtex
@article{zheng2021scattering,
  title={De-scattering with excitation patterning enables rapid wide-field imaging through scattering media},
  author={Zheng, Cheng and Park, Jong Kang and Yildirim, Murat and Boivin, Josiah R and Xue, Yi and Sur, Mriganka and So, Peter TC and Wadduwage, Dushan N},
  journal={Science advances},
  volume={7},
  number={28},
  eid={eaay5496},
  year={2021},
  doi={10.1126/sciadv.aay5496}
}
```

### DEEP-squared (2023)

```bibtex
@article{wijethilake2023deep,
  title={{DEEP}-squared: deep learning powered de-scattering with excitation patterning},
  author={Wijethilake, Navodini and Anandakumar, Mithunjha and Zheng, Cheng and So, Peter TC and Yildirim, Murat and Wadduwage, Dushan N},
  journal={Light: Science and Applications},
  volume={12},
  number={1},
  eid={228},
  year={2023},
  doi={10.1038/s41377-023-01248-6}
}
```

---

## Relationship between the two papers

The two papers are **directly connected**: DEEPsquared builds upon DEEP.

### DEEP (2021)

- Introduces a **physics-based computational imaging method**
- Uses **structured illumination** and **wide-field detection**
- Formulates image recovery as an **inverse optimization problem**
- Requires **128–256 illumination patterns** and **iterative reconstruction**

### DEEP-squared (2023)

- Extends DEEP by replacing optimization with **deep learning**
- Learns the inverse mapping (X = f⁻¹(y))
- Uses a **U-Net-based neural network** with attention mechanisms
- Reduces required measurements to **~32 patterns** (~10× improvement)

### Key insight

- DEEP defines the **forward imaging model**: \(y = f(X)\)
- DEEP-squared learns the **inverse mapping**: (X = f⁻¹(y))

**Therefore:** DEEP-squared depends on DEEP for the physics, forward model, and training data generation, and improves reconstruction using deep learning.

---

## Final takeaway

- **DEEP** treats scattering as an **encoding problem**
- **DEEPsquared** treats reconstruction as a **learning problem**

Together, they support **fast, high-resolution imaging through scattering biological tissue**.
