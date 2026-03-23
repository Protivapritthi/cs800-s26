# Assignment 5: Literature Review Part 2
CS 800 – Research Methods, Spring 2026  
Student: Protiva Das

## Assignment Description

This assignment analyzes the relationship between two research papers in the area of LLM security and multi-turn jailbreak attacks. The goal is to understand how a newer work builds upon and improves the limitations of an earlier framework.

The selected papers are:

- **NEXUS (2025)** – Introduces a structured framework for multi-turn jailbreak attacks using semantic exploration.
- **Mastermind (2026)** – Extends this direction by introducing a knowledge-driven, adaptive, and planning-based attack framework.

The presentation focuses on:
- understanding multi-turn jailbreak attacks,
- the NEXUS framework,
- the Mastermind framework, and
- a clear explanation of how Mastermind builds upon NEXUS.

## Repository Structure

    .
    ├── README.md
    ├── Protiva_A5 Presentation.pptx
    ├── Mastermind.pdf
    └── paper5_NEXUS_marked.pdf

## Papers

### 1. NEXUS (Paper A)
**Title:** NEXUS: Network Exploration for Exploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks  
**Authors:** Javad Rafiei Asl, Sidhant Narula, Mohammad Ghasemigol, Eduardo Blanco, and Daniel Takabi  
**Venue:** EMNLP, 2025

### 2. Mastermind (Paper B)
**Title:** Knowledge-Driven Multi-Turn Jailbreaking on Large Language Models  
**Authors:** Songze Li, Ruishi He, Xiaojun Jia, Jun Wang, and Zhihui Fu  
**Venue:** arXiv, 2026

## Relationship Between the Two Papers

The two papers are directly related because both study multi-turn jailbreak attacks on large language models. Mastermind builds upon the research direction established by NEXUS and improves several of its limitations.

### NEXUS (Paper A)
- Introduces a structured framework for multi-turn jailbreak attacks.
- Models the jailbreak process as exploration of adversarial query space.
- Uses ThoughtNet, Simulator, and Traverser for attack generation.
- Focuses on systematic, search-based attack strategies.

### Mastermind (Paper B)
- Extends NEXUS by introducing a knowledge-driven framework.
- Uses Planner–Executor–Controller architecture.
- Enables learning, long-term planning, and adaptive strategy refinement.
- Focuses on dynamic and evolving attack strategies.

### Key Relationship
- NEXUS explores the adversarial space using structured search.
- Mastermind improves this by adding learning, planning, and adaptation.
- NEXUS = search-based approach, Mastermind = learning-based approach.

### Final Insight
From structured exploration (NEXUS)  
to adaptive strategy learning (Mastermind)

## Slides Presentation

Google Slides Link: https://docs.google.com/presentation/d/1Z7iLlR5hQIqJqf-fu8mHTYBhDHGH9Rukb5GuLZTLghM/edit?usp=sharing

## BibTeX Entries

### NEXUS (2025)

    @inproceedings{asl2025nexus,
      author    = {Asl, Javad Rafiei and Narula, Sidhant and Ghasemigol, Mohammad and Blanco, Eduardo and Takabi, Daniel},
      title     = {{NEXUS}: Network Exploration for Exploiting Unsafe Sequences in Multi-Turn {LLM} Jailbreaks},
      booktitle = {Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP)},
      pages     = {24267--24295},
      year      = {2025}
    }

### Mastermind (2026)

    @techreport{li2026knowledge,
      author      = {Li, Songze and He, Ruishi and Jia, Xiaojun and Wang, Jun and Fu, Zhihui},
      title       = {Knowledge-Driven Multi-Turn Jailbreaking on Large Language Models},
      institution = {arXiv},
      year        = {2026},
      number      = {arXiv:2601.05445}
    }
