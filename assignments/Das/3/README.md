# Assignment 3: Reading Papers
CS 800 Research Methods, Spring 2026  
**Name:** Protiva Das

This submission contains five papers from my research area (**LLM security, privacy, and adversarial robustness**), each with **Keshav’s 1st-pass summary** (**problem, approach, contributions**), **reference**, **DOI link**, **BibTeX entry**, and a **marked-up PDF** highlighting the relevant sections.

---

## **Directory structure**

assignments/Das/3/  
├── README.md  
├── A3_papers_marked/  
│   ├── paper1_GuardAgent_marked.pdf  
│   ├── paper2_HiddenNoMore_marked.pdf  
│   ├── paper3_SecureCodeGen_marked.pdf  
│   ├── paper4_BackdoorSurvey_marked.pdf  
│   └── paper5_NEXUS_marked.pdf  
└── paper_images/  
    ├── paper 1.png  
    ├── paper 2.png  
    ├── paper 3.png  
    ├── paper 4.png  
    └── paper 5.png  

---

## **Paper 1: GuardAgent – Safeguard LLM Agents via Knowledge-Enabled Reasoning**

**Reference:**  
Xiang, Z., Zheng, L., Li, Y., Hong, J., Li, Q., Xie, H., ... & Li, B. (2025, July). Guardagent: safeguard LLM agents via knowledge-enabled reasoning. In ICML 2025 workshop on computer use agents.

**DOI:**  
https://arxiv.org/abs/2406.09187

**BibTeX:**  
@inproceedings{xiang2025guardagent,  
  title={Guardagent: safeguard LLM agents via knowledge-enabled reasoning},  
  author={Xiang, Zhen and Zheng, Linzhi and Li, Yanjie and Hong, Junyuan and Li, Qinbin and Xie, Han and Zhang, Jiawei and Xiong, Zidi and Xie, Chulin and Bastian, Nathaniel D and others},  
  booktitle={ICML 2025 workshop on computer use agents},  
  year={2025}  
}

**1st pass (Keshav):**

**Problem:**  
LLM agents can autonomously execute actions using tools, but existing safety mechanisms are either hard-coded or limited to text moderation, making them unsuitable for enforcing flexible, action-level safety and privacy policies.

**Approach:**  
The authors propose GuardAgent, a separate LLM-based guard agent that converts safety requirements into action plans, generates executable guardrail code, and enforces safety by executing the code on target agent logs using memory-supported reasoning.

**Contributions:**  
- Introduces the first guardrail agent designed to protect other LLM agents.  
- Uses code generation and execution to enforce safety more reliably than text-only guardrails.  
- Proposes two benchmarks (EICU-AC and Mind2Web-SC) and achieves high guardrail accuracy.

**Screenshot (Page 1):**  
![](paper_images/paper%201.png)

**Marked-up PDF:**  
[A3_papers_marked/paper1_GuardAgent_marked.pdf](A3_papers_marked/paper1_GuardAgent_marked.pdf)

---

## **Paper 2: Hidden No More – Attacking and Defending Private Third-Party LLM Inference**

**Reference:**  
Pal, A., Thomas, R. K., Zahran, L., Choi, E., Potti, A., & Goldblum, M. (2025). Hidden no more: attacking and defending private third-party LLM inference. In ICLR 2025 workshop on building trust in language models and applications.

**DOI:**  
https://openreview.net/forum?id=QfD9P9IIoz

**BibTeX:**  
@inproceedings{pal2025hidden,  
  title={Hidden no more: attacking and defending private third-party LLM inference},  
  author={Pal, Arka and Thomas, Rahul Krishna and Zahran, Louai and Choi, Erica and Potti, Akilesh and Goldblum, Micah},  
  booktitle={ICLR 2025 workshop on building trust in language models and applications},  
  year={2025}  
}

**1st pass (Keshav):**

**Problem:**  
Third-party LLM inference services expose sensitive user prompts, and existing privacy-preserving defenses incorrectly assume that hidden states cannot be reversed.

**Approach:**  
The authors design a hidden-state reconstruction attack that recovers user prompts with near-perfect accuracy and propose Cascade, a token-sharded multi-party inference scheme to prevent reconstruction.

**Contributions:**  
- Demonstrates a practical and highly accurate hidden-state reconstruction attack.  
- Shows that permutation- and noise-based defenses are insecure.  
- Proposes Cascade as an efficient privacy-preserving defense.

**Screenshot (Page 2):**  
![](paper_images/paper%202.png)

**Marked-up PDF:**  
[A3_papers_marked/paper2_HiddenNoMore_marked.pdf](A3_papers_marked/paper2_HiddenNoMore_marked.pdf)

---

## **Paper 3: How Secure is Secure Code Generation? Adversarial Prompts Put LLM Defenses to the Test**

**Reference:**  
Tessa, M., Olatunji, I. E., War, A., Klein, J., & Bissyandé, T. F. (2026). How Secure is Secure Code Generation? Adversarial Prompts Put LLM Defenses to the Test. arXiv preprint arXiv:2601.07084.

**DOI:**  
https://arxiv.org/abs/2601.07084

**BibTeX:**  
@article{tessa2026secure,  
  title={How Secure is Secure Code Generation? Adversarial Prompts Put LLM Defenses to the Test},  
  author={Tessa, Melissa and Olatunji, Iyiola E and War, Aicha and Klein, Jacques and Bissyand{\'e}, Tegawend{\'e} F},  
  journal={arXiv preprint arXiv:2601.07084},  
  year={2026}  
}

**1st pass (Keshav):**

**Problem:**  
Secure code generation methods claim to prevent vulnerable outputs, but their robustness under realistic adversarial prompts is unclear.

**Approach:**  
The authors conduct a systematic adversarial audit using realistic prompt perturbations and jointly evaluate security and functionality.

**Contributions:**  
- Performs the first adversarial robustness audit of secure code generation methods.  
- Shows static analyzers overestimate security.  
- Proposes best practices for robust evaluation.

**Screenshot (Page 3):**  
![](paper_images/paper%203.png)

**Marked-up PDF:**  
[A3_papers_marked/paper3_SecureCodeGen_marked.pdf](A3_papers_marked/paper3_SecureCodeGen_marked.pdf)

---

## **Paper 4: Backdoor Attacks and Countermeasures in Natural Language Processing Models: A Comprehensive Security Review**

**Reference:**  
Cheng, P., Wu, Z., Du, W., Zhao, H., Lu, W., & Liu, G. (2025). Backdoor attacks and countermeasures in natural language processing models: A comprehensive security review. IEEE Transactions on Neural Networks and Learning Systems.

**DOI:**  
https://arxiv.org/abs/2309.06055

**BibTeX:**  
@article{cheng2025backdoor,  
  title={Backdoor attacks and countermeasures in natural language processing models: A comprehensive security review},  
  author={Cheng, Pengzhou and Wu, Zongru and Du, Wei and Zhao, Haodong and Lu, Wei and Liu, Gongshen},  
  journal={IEEE Transactions on Neural Networks and Learning Systems},  
  year={2025},  
  publisher={IEEE}  
}

**1st pass (Keshav):**

**Problem:**  
Backdoor attacks threaten NLP models and LLMs, but prior surveys lack a unified and up-to-date view.

**Approach:**  
The paper systematically surveys backdoor attacks and defenses across training and deployment stages.

**Contributions:**  
- Provides a unified taxonomy of backdoor attacks.  
- Categorizes defenses into sample and model inspection.  
- Identifies open challenges and future directions.

**Screenshot (Page 4):**  
![](paper_images/paper%204.png)

**Marked-up PDF:**  
[A3_papers_marked/paper4_BackdoorSurvey_marked.pdf](A3_papers_marked/paper4_BackdoorSurvey_marked.pdf)

---

## **Paper 5: NEXUS: Network Exploration for eXploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks**

**Reference:**  
Asl, J. R., Narula, S., Ghasemigol, M., Blanco, E., & Takabi, D. (2025, November). NEXUS: Network Exploration for eXploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks. In Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing (pp. 24278-24306).

**DOI:**  
https://arxiv.org/abs/2510.03417

**BibTeX:**  
@inproceedings{asl2025nexus,  
  title={NEXUS: Network Exploration for eXploiting Unsafe Sequences in Multi-Turn LLM Jailbreaks},  
  author={Asl, Javad Rafiei and Narula, Sidhant and Ghasemigol, Mohammad and Blanco, Eduardo and Takabi, Daniel},  
  booktitle={Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing},  
  pages={24278--24306},  
  year={2025}  
}

**1st pass (Keshav):**

**Problem:**  
Multi-turn jailbreak attacks bypass LLM safety mechanisms by distributing malicious intent across benign interactions.

**Approach:**  
The authors propose NEXUS, a modular framework that builds semantic attack networks and refines attack chains using feedback-driven simulation.

**Contributions:**  
- Introduces a structured framework for multi-turn jailbreak attacks.  
- Proposes ThoughtNet and feedback-driven refinement.  
- Achieves higher attack success rates and diversity.

**Screenshot (Page 5):**  
![](paper_images/paper%205.png)

**Marked-up PDF:**  
[A3_papers_marked/paper5_NEXUS_marked.pdf](A3_papers_marked/paper5_NEXUS_marked.pdf)

---

## **Video walkthrough**

A short YouTube video walking through the papers and discussing the 1st-pass highlights:

**Video Link:** https://youtu.be/spAzK32RXmI
