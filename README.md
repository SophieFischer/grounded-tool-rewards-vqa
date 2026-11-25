# Grounded Tool Rewards for Agentic Vision-Language Models

## 📰 News

* **2026/11**: Our paper has been accepted to [EACL 2027](https://2027.eacl.org) (Main)! 🎉

## 📖 Overview

Agentic vision-language models can leverage external tools to overcome perceptual limitations in visual question-answering (VQA).
Current reinforcement learning methods do not account for the fact that not every VQA question requires a tool, and cannot distinguish between questions that coincide with a tool call and those that require the tool output.
We therefore introduce verified tool labels, by exhaustively searching every tool set (zoom, depth, detection, pointing, captioning) to find which tool sets actually fix a wrong answer.
We use these model-specific verified labels to train the vision-language model policy to call tools more selectively.

1. **Verified labels.** For every question, the tool sets whose search branch answers correctly (`plausible_plans_list`) and a `hardness_label` (`easy`, `hard`, `unsolved`).
2. **Training.** GRPO with a reward grounded in the verified tool sets (R_agentic, R_total), a reasoning-only variant (R_think), and SFT on tool-use traces built from the same labels.
3. **Evaluation.** Smart-routing evaluation on CV-Bench, V*, BLINK and RealWorldQA, plus zero-shot, no-image, random-answer and all-tools baselines.

## 🏗️ Installation + Code

COMING SOON
