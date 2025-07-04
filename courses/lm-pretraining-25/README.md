# Pretraining LMs (UdS; WiSe 25/26)

## Description

Correct pretraining of LLMs is critical for optimal downstream performance. Unfortunately, the prohibitive size of SoTA models means that many students never get the chance to gain hands-on experience in this area. Furthermore, the actual pretraining process is often hidden in the appendix or glossed over entirely in research papers and technical reports (especially for propreitary models), making it extremely difficult to gain insight into good practices.

The goal of this software project is to rectify this state of affairs: students will gain hands-on experience pretraining an LLM from scratch, evaluating their pretrained model, analyzing the results of these evaluations, and making informed, iterative improvements to the architecture and/or pretraining procedure based on these analyses&mdash;all on a highly constrained time and resource budget. In groups of 1-3, students will choose a baseline model architecture, pretraining dataset, and set of validation tasks. The overall objective of this course is to gradually improve the model's performance on the validation tasks, by iteratively tweaking the model architecture and pretraining pipeline.

## Prerequisites

This course is geared towards Master's students who have experience with either PyTorch or Tensorflow. You should also be familiar with the details of transformer architectures (multi-head attention, etc.) and basic preprocessing methods such as data de-duplication and tokenization.

## Information

**Instructor:** [Michael Sullivan](https://mjs227.github.io/home/)
- msullivan@lst.uni-saarland.de

**Time/Location:** Building C7.2, Room 1.04 (time varies per team) 

## Schedule

This course will be divided into five phases throughout the semester.

### Phase 1: Establishing a Baseline

In this phase, you will find a pretraining corpus (and preprocess the data), and find/create a set of 3-5 validation tasks to use to evaluate your model. These validation tasks should be relatively small (for fast evaluation), and *not* require any additional fine-tuning: the objective of this course is to improve performance *solely* through tweaks to the model architecture and pretraining procedure.

You will then choose a *small* model architecure (e.g. GPT-2) to use as your baseline: we have a very limited compute budget, so your model must be able to train relatively quickly (and fit in GPU memory!). You will implement this architecure *from scratch* in your chosen library (PyTorch or Tensorflow), in order to be able to easily make modifications to the architecture in later stages of the project.

You task will then be to pretrain this model on your dataset, making informed choices regarding hyperparameter configuration. Finally, you will evaluate the pretrained model on your validation tasks.

### Phase 2: Analysis (Part 1)

Your task in this phase will then be to analyze the results of Phase 1, with a particular emphasis on data visualization. You will inspect various metrics across pretraining (e.g. loss) and the validation tasks, with the goal of identifying weaknesses in your pretraining procedure.

### Phase 3: Propose and Evaluate Changes

Based on your analysis in Phase 2, you will then propose (and justify) changes to the model architecture and pretraining pipeline. Your task in this phase is to iteratively improve your model, making small changes at each iteration to disentagle the effects of each particular modification on downstream performance. Note that you will be operating under a highly constrained time and resource budget: a brute-force grid search across all of your proposed changes will not work! You will need to make informed decisions at each step of this process, carefully considering the tradeoff between the costs and benefits of evaluating a new change to the architecture/pipeline.

I *highly* recommend applying the techniques of the [Google Research Tuning Playbook](https://github.com/google-research/tuning_playbook) to this phase: this document is full of extremely useful tips and methods for systematically and scientifically improving model performance under a constrained compute budget.

### Phase 4: Analysis (Part 2)

In this phase, you will apply the techniques that you implemented in Phase 2 to the experiments that you ran in Phase 3. Which metrics improved? Which got worse? Why?

### Phase 5: Final Report

You will then write up a final report on your findings. Describe your baseline model and the analysis that you conducted in Phase 2. Discuss the modifications that you implemented in Phase 3, and justify them using your Phase 2 analysis and prior research in this area. Use your Phase 4 analysis to demonstate the benefits (and limitations) of these modifications. This report should be in ACL format, and limited to a maximum of eight pages (excluding references and appendix).

The final report and all code/materials used in Phases 1-4 will be due by March 21, 2025.

## Evaluation

```
Project Work (Phases 1-4): 65%
Final Report (Phase 5): 35%
```
