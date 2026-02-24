# Assignment 3: Reading Papers
CS 800 Research Methods, Spring 2026  
**Name:** Protiva Das

This submission contains five papers from my research area (**LLM security, privacy, and adversarial robustness**), each with **Keshav’s 1st-pass summary** (problem, approach, contributions), **reference**, **DOI link**, **BibTeX entry**, and a **marked-up PDF** highlighting the relevant sections.

---

## Directory structure

assignments/Das/3/
│
├── README.md
│
├── A3_papers_marked/
│ ├── paper1_GuardAgent_marked.pdf
│ ├── paper2_HiddenNoMore_marked.pdf
│ ├── paper3_SecureCodeGen_marked.pdf
│ ├── paper4_BackdoorSurvey_marked.pdf
│ └── paper5_NEXUS_marked.pdf
│
└── paper_images/
├── paper 1.png
├── paper 2.png
├── paper 3.png
├── paper 4.png
└── paper 5.png


---

## Paper 1: GuardAgent – Safeguard LLM Agents via Knowledge-Enabled Reasoning

**Reference:**  
Zhen Xiang, Linzhi Zheng, Yanjie Li, et al. *GuardAgent: Safeguard LLM Agents via Knowledge-Enabled Reasoning.* ICML Workshop on Computer-Use Agents, 2025.

**DOI:**  
https://doi.org/10.48550/arXiv.2406.XXXX

```bibtex
@article{xiang2025guardagent,
  title={GuardAgent: Safeguard LLM Agents via Knowledge-Enabled Reasoning},
  author={Xiang, Zhen and Zheng, Linzhi and Li, Yanjie and others},
  journal={arXiv preprint},
  year={2025}
}

1st pass (Keshav):

Problem:
LLM agents can autonomously execute actions using tools, but existing safety mechanisms are either hard-coded or limited to text moderation, making them unsuitable for enforcing flexible, action-level safety and privacy policies.

Approach:
The authors propose GuardAgent, a separate LLM-based guard agent that converts safety requirements into action plans, generates executable guardrail code, and enforces safety by executing the code on target agent logs using memory-supported reasoning.

Contributions:

Introduces the first guardrail agent designed to protect other LLM agents.

Uses code generation and execution to enforce safety more reliably than text-only guardrails.

Proposes two benchmarks (EICU-AC and Mind2Web-SC) and achieves 83–98% guardrail accuracy.

Screenshot (Page 1):


Marked-up PDF:
A3_papers_marked/paper1_GuardAgent_marked.pdf

Paper 2: Hidden No More – Attacking and Defending Private Third-Party LLM Inference

Reference:
Rahul Thomas, Louai Zahran, Erica Choi, et al. Hidden No More: Attacking and Defending Private Third-Party LLM Inference. ICLR Building Trust Workshop, 2025.

DOI:
https://doi.org/10.48550/arXiv.2404.XXXX

@article{thomas2025hidden,
  title={Hidden No More: Attacking and Defending Private Third-Party LLM Inference},
  author={Thomas, Rahul and Zahran, Louai and Choi, Erica and others},
  journal={arXiv preprint},
  year={2025}
}

1st pass (Keshav):

Problem:
Third-party LLM inference services expose sensitive user prompts, and existing privacy-preserving defenses incorrectly assume that hidden states cannot be reversed.

Approach:
The authors design a hidden-state reconstruction attack that recovers user prompts with near-perfect accuracy and propose Cascade, a token-sharded multi-party inference scheme that prevents reconstruction while remaining efficient.

Contributions:

Demonstrates a practical and highly accurate hidden-state reconstruction attack.

Shows that permutation- and noise-based defenses are insecure.

Proposes Cascade as an efficient and robust privacy-preserving defense.

Screenshot (Page 1):


Marked-up PDF:
A3_papers_marked/paper2_HiddenNoMore_marked.pdf

Paper 3: How Secure is Secure Code Generation? Adversarial Prompts Put LLM Defenses to the Test

Reference:
Melissa Tessa, Iyiola E. Olatunji, Aicha War, et al. How Secure is Secure Code Generation? ACM, 2026.

DOI:
https://doi.org/10.48550/arXiv.2601.07084

@article{tessa2026secure,
  title={How Secure is Secure Code Generation? Adversarial Prompts Put LLM Defenses to the Test},
  author={Tessa, Melissa and Olatunji, Iyiola and War, Aicha and others},
  journal={arXiv preprint arXiv:2601.07084},
  year={2026}
}

1st pass (Keshav):

Problem:
Secure code generation methods claim to prevent vulnerable outputs, but their robustness under realistic adversarial prompts and joint security-functionality evaluation is unclear.

Approach:
The authors conduct a systematic adversarial audit using realistic prompt perturbations and evaluate security and functionality jointly under a unified framework.

Contributions:

Performs the first adversarial robustness audit of secure code generation methods.

Shows that static analyzers overestimate security and many outputs are non-functional.

Proposes best practices for robust secure code generation evaluation.

Screenshot (Page 1):


Marked-up PDF:
A3_papers_marked/paper3_SecureCodeGen_marked.pdf

Paper 4: Backdoor Attacks and Countermeasures in NLP Models – A Comprehensive Security Review

Reference:
Pengzhou Cheng, Zongru Wu, Wei Du, et al. Backdoor Attacks and Countermeasures in NLP Models. IEEE Transactions on Neural Networks and Learning Systems, 2025.

DOI:
https://doi.org/10.1109/TNNLS.2025.3540303

@article{cheng2025backdoor,
  title={Backdoor Attacks and Countermeasures in Natural Language Processing Models: A Comprehensive Security Review},
  author={Cheng, Pengzhou and Wu, Zongru and Du, Wei and others},
  journal={IEEE Transactions on Neural Networks and Learning Systems},
  year={2025}
}

1st pass (Keshav):

Problem:
Backdoor attacks threaten NLP models and LLMs, but prior surveys lack a unified and up-to-date view across modern training and deployment pipelines.

Approach:
The paper systematically surveys backdoor attacks and defenses by categorizing them based on attacker capability and model stage.

Contributions:

Provides a unified taxonomy of backdoor attacks across NLP and LLMs.

Categorizes defenses into sample inspection and model inspection.

Identifies benchmarks, gaps, and future research directions.

Screenshot (Page 1):


Marked-up PDF:
A3_papers_marked/paper4_BackdoorSurvey_marked.pdf

Paper 5: NEXUS – Network Exploration for Exploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks

Reference:
Javad Rafiei Asl, Sidhant Narula, Mohammad Ghasemigol, et al. NEXUS: Network Exploration for Exploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks. EMNLP, 2025.

DOI:
https://doi.org/10.48550/arXiv.2410.XXXX

@article{rafiei2025nexus,
  title={NEXUS: Network Exploration for Exploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks},
  author={Rafiei Asl, Javad and Narula, Sidhant and Ghasemigol, Mohammad and others},
  journal={arXiv preprint},
  year={2025}
}

1st pass (Keshav):

Problem:
Multi-turn jailbreak attacks bypass LLM safety mechanisms by distributing malicious intent across benign interactions, and existing methods lack systematic exploration and refinement.

Approach:
The authors propose NEXUS, a modular framework that builds semantic attack networks, refines queries using feedback-driven simulation, and adaptively executes optimized jailbreak chains.

Contributions:

Introduces a structured framework for systematic multi-turn jailbreak attacks.

Proposes ThoughtNet and feedback-driven refinement for attack generation.

Achieves higher attack success rates and diversity across multiple LLMs.

Screenshot (Page 1):


Marked-up PDF:
A3_papers_marked/paper5_NEXUS_marked.pdf

Video walkthrough

A short YouTube video walking through the papers and discussing the 1st-pass highlights:

Video Link: PASTE YOUR UNLISTED YOUTUBE LINK HERE
