# Assignment 5, Literature Review, Part 2

**CS 800 Research Methods, Spring 2026**
**Student:** Yamini Chitikela

## Description

This assignment explores the relationship between two research papers in the field of **graph neural network expressiveness and generalization via graph homomorphism**. The goal is to understand how a newer paper builds upon an existing foundational work.

- **Base Paper:** Li et al. 2024 — *Generalization of Graph Neural Networks through the Lens of Homomorphism*
- **Second Paper:** Li et al. 2025 — *Towards Bridging Generalization and Expressivity of Graph Neural Networks*

The focus is on identifying how the second paper **extends and builds directly on** the framework introduced in the first paper.

## Directory and File Structure

The files for this assignment are organized as follows:

- `README.md`: This file, documenting the assignment submission.
- [papers](./papers/): Directory containing the PDF copies of the two research papers presented in this literature review.

## BibTeX Entries

- [Paper 1](./papers/paper1.pdf): Generalization of Graph Neural Networks through the Lens of Homomorphism

```bibtex
@misc{li2024generalization,
  title        = {Generalization of Graph Neural Networks through the Lens of Homomorphism},
  author       = {Li, Shouheng and Kim, Dongwoo and Wang, Qing},
  year         = {2024},
  howpublished = {arXiv:2403.06079},
  url          = {https://arxiv.org/abs/2403.06079}
}
```

- [Paper 2](./papers/paper2.pdf): Towards Bridging Generalization and Expressivity of Graph Neural Networks

```bibtex
@inproceedings{li2025towards,
  title     = {Towards Bridging Generalization and Expressivity of Graph Neural Networks},
  author    = {Li, Shouheng and Geerts, Floris and Kim, Dongwoo and Wang, Qing},
  booktitle = {The Thirteenth International Conference on Learning Representations},
  year      = {2025},
  url       = {https://openreview.net/forum?id=BOQpRtI4F5}
}
```

## Relationship Between the Two Papers

### Li et al. 2024 — Base Paper

- Introduces the use of **graph homomorphism counts** as GNN features
- Derives the first **generalization bounds tied to graph structure** — prior bounds were graph-agnostic
- Shows that the structural complexity of the graph family (measured via homomorphism) directly controls how well a GNN generalizes
- Designed for:
  - Provable generalization guarantees on graph-structured data
  - Structure-aware learning on graph families
- **Limitation it leaves open:** Expressiveness is not addressed — generalization and expressiveness remain disconnected

### Li et al. 2025 — Second Paper (ICLR 2025)

- Builds **directly on Li et al. 2024** by using the same homomorphism-based framework as its foundation
- Extends the 2024 work to:
  - Formally connect **expressiveness** to the homomorphism framework
  - Show that the same counts that bound generalization also induce an **expressiveness hierarchy**
  - Quantify the tradeoff between expressiveness and generalization in a single unified theory
- Introduces:
  - A unified homomorphism-based framework covering both properties
  - Formal proof that increasing pattern family size simultaneously increases expressiveness and loosens generalization bounds
- New co-author **Floris Geerts** brings expressiveness expertise — he also co-authored the foundational Barceló et al. 2021 paper on local graph parameters

### Key Relationship

- **Direct Foundation**
  - Paper 2 uses Paper 1's homomorphism feature representation and generalization bound as its starting point — not background, but scaffolding
- **Extension to Expressiveness**
  - Paper 1 only addressed generalization — Paper 2 brings expressiveness into the same framework
- **Unified Theory**
  - For the first time, a single framework formally captures both GNN properties together
- **Quantifiable Tradeoff**
  - Paper 2 makes the expressiveness vs. generalization tradeoff mathematically precise — something Paper 1 could not do alone
- **Same Research Group**
  - Li, Kim, and Wang are authors on both papers — Paper 2 is a direct continuation of their own prior work

## Slides Presentation

**Google Slides Link:** (https://docs.google.com/presentation/d/10mGF6sHYWGTO2GSrgVl3p4B7-wtahmWI/edit?slide=id.p1#slide=id.p1)
