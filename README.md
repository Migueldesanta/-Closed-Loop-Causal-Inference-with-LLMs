# Closed-Loop Causal Inference with LLMs

This repository supports a research project exploring **closed-loop causal inference** in political science using large language models (LLMs). The goal is to test whether a single LLM—or a modular prompt-based pipeline—can autonomously conduct three key stages of a causal experiment: **treatment generation**, **(optional) response simulation**, and **causal reasoning**, all without human-labeled data.

---

## 🔁 Framework Overview

1. **Treatment Generation**  
   The LLM generates political stimuli (e.g. framing, tone, or ideological variants).

2. **(Optional) Simulated Response**  
   The LLM simulates responses by virtual subjects with different political traits.

3. **Causal Reasoning**  
   The LLM evaluates whether treatment variation likely caused differences in responses, based on principles like counterfactuals and confounding.

4. **Feedback to Treatment Design**  
   Reasoning outcomes (e.g. “no effect”) can be used to refine the next generation of treatments — closing the loop.

---

## 📚 Literature Review

This project is inspired by the following detailed insights:

- **Yu et al. (2024)** distinguish between LLMs as “reasoning engines” vs. “data tools.” This project tests LLMs as full reasoning agents, conducting causal inference end-to-end.

- **Ma (2025)** highlights that LLMs can simulate social science pipelines if broken into modular stages (design → simulate → infer). Our framework instantiates this pipeline and evaluates it experimentally.

- **Liu et al. (2025)** argue LLMs are powerful collaborators in causal studies. We push this by removing the human and asking whether LLMs alone can produce usable insights.

- **Sgouritsa et al. (2024)** show LLMs can be guided through causal structure learning using question decomposition. We borrow this principle for structured reasoning prompts.

- **Manning et al. (2024)** use LLMs to generate and test social science hypotheses. Our project complements this by explicitly targeting the causal chain of influence, not just descriptive patterns.

---

## 🧪 Evaluation Strategy

We assess the pipeline across three dimensions:

- **Plausibility**: Are the generated treatments realistic and comparable to human-designed messages?
- **Sensitivity**: Do different treatments elicit different simulated responses?
- **Causal Correctness**: Do the reasoning outputs reflect correct counterfactual logic and avoid common fallacies?

Optional human evaluation may assess LLM outputs qualitatively. Alternatively, comparison to pre-labeled toy datasets (e.g. known cause-effect examples) provides structure.

---

## 🧠 Key Contributions

- An **automated causal experiment loop** that removes the human from design + inference.
- **Prompt-based modular design** that can be extended to new political topics.
- Early proof-of-concept for **LLMs as political science researchers**.

---
## 📚 References

- Yu, L. et al. (2024). *Improving Causal Reasoning in Large Language Models: A Survey*. arXiv:2410.16676v1.
- Ma, J. (2025). *Causal Inference with Large Language Models: A Survey*.
- Liu, Y. et al. (2025). *Large Language Models and Causal Inference in Collaboration: A Survey*.
- Sgouritsa, A. et al. (2024). *Prompting LLMs for Sub-question Guided Causal Discovery*. arXiv:2412.13952.
- Manning, B. et al. (2024). *Social Science in Silico: Generating and Testing Theories with LLMs*.

