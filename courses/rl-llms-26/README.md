# Reinforcement Learning for LLMs (UdS; WiSe 25/26)

## Description

In this seminar, we delve into reinforcement learning for LLMs, with a particular focus on reinforcement learning with verifiable reward (RLVR): the learning paradigm powering current advances in frontier reasoning LLMs. The course is divided into three units: in the Introduction, we will build up our understanding of RL algorithms, from basic policy-gradient methods (e.g. REINFORCE) to current, cutting edge approaches (e.g. DAPO). In the Reward/Credit Assignment unit, we will study the effect of reward on RL training pipelines, and the difficulties of fine-grained credit assignment in long-horizon reasoning training. Finally, we will discuss Training Dynamics: what behavior does RL incentivize, and by what mechanisms?

## Prerequisites

This course assumes a solid background in ML and LLMs: in particular, you should be familiar with transformer architectures and common methods/terminology in ML/NLP, and have a solid grasp on the mathematics behind LLM training.

## Information

**Instructor:** [Michael Sullivan](https://mjs227.github.io/home/) 
- Email: msullivan@lst.uni-saarland.de

**Time/Location:** Mon 12:15 - 13:45; Building C7.2, Room 1.14

## Format/Requirements

Each week, we will meet to discuss the assigned reading (see *Schedule/Reading List* below). All students are expected to *participate in the discussion in every class meeting*  (this includes asking questions).

### Discussion Leader

At the beginning of the semester, each student will choose a reading for which they will create a presentation and lead the discussion ("Discussion Leader"). If you do not reach out to me to chose a reading, I will randomly assign you a paper. The Discussion Leader will:

- **Summarize**: Discuss the authors' approach/methods, main findings, and any relevant background on the topic
- **Critically analyze**: What is your opinion of the methods/findings of the paper? What should (or shouldn't) have been included? What limitations does this approach have?
- **Field questions**: While you are *not* expected to cover every minute detail of the reading in your presentation, you *should* know the paper well enough to be able to answer any questions your classmates might have (within reason, of course!).

## Evaluation

For students taking the course for 4 credits:
```
Participation in class discussions: 50%
Discussion Leader: 50%
```

For students taking the course for 7 credits:
```
Participation in class discussions: 30%
Discussion Leader: 30%
Term paper: 40%
```

## Schedule/Reading List

| Topic | Date | Reading | Discussion Leader |
| :--- | :--- | :--- | :--- |
| Introduction | Oct. 19 | None (logistics and scheduling)<br>**NOTE: CLASS ONLINE** (Michael at RTG retreat) | Michael |
| Introduction | Oct. 26 | **NO CLASS** (Michael at EMNLP) | - |
| Introduction | Nov. 2 | [A First-Principles Derivation of LLM Policy Optimization](https://arxiv.org/pdf/2606.16733) (Part I) | Michael |
| Introduction | Nov. 9 | [DAPO](https://arxiv.org/pdf/2503.14476) & [DeepSeekMath](https://arxiv.org/pdf/2402.03300) (Sec. 4)  | TBD |
| Reward/Credit Assignment | Nov. 16 | [Demystifying Long Chain-of-Thought Reasoning in LLMs](https://arxiv.org/pdf/2502.03373) | TBD |
| Reward/Credit Assignment | Nov. 23 | [Reward Under Attack](https://arxiv.org/pdf/2603.06621) | TBD |
| Reward/Credit Assignment | Nov. 30 | [VinePPO](https://arxiv.org/pdf/2410.01679) | TBD |
| Reward/Credit Assignment | Dec. 7 | [GRPO is Secretly a Process Reward Model](https://arxiv.org/pdf/2509.21154) | TBD |
| Training Dynamics | Dec. 14 | [The Entropy Mechanism of Reinforcement Learning for Reasoning Language Models](https://arxiv.org/pdf/2505.22617) | TBD |
| Break | Dec. 21 | **NO CLASS** (break) | - |
| Break | Dec. 28 | **NO CLASS** (break) | - |
| Training Dynamics | Jan. 4 | [RL's Razor](https://proceedings.iclr.cc/paper_files/paper/2026/file/618c95f4557c15b253fb0e6f548ea0c0-Paper-Conference.pdf) | TBD |
| Training Dynamics | Jan. 11 | **NO CLASS** (Michael in US) | - |
| Training Dynamics | Jan. 18 | [SFT Memorizes, RL Generalizes](https://openreview.net/pdf?id=d3E3LWmTar) | TBD |
| Training Dynamics | Jan. 25 | [Does Reinforcement Learning Really Incentivize Reasoning Capacity in LLMs Beyond the Base Model?](https://proceedings.neurips.cc/paper_files/paper/2025/file/537d5aa768c2d534016a4d06f87bc8fb-Paper-Conference.pdf) | TBD |
| Training Dynamics | Feb. 1 | [ProRL](https://proceedings.neurips.cc/paper_files/paper/2025/file/1a22b912945fb7c0bdd079e792b31b6f-Paper-Conference.pdf) | TBD |

## Term Papers

Students taking the course for 7 credits will be expected to write a survey paper on one of the topics discussed in class (or&mdash;with my approval&mdash;another topic in RL for LLMs). Your task is to take a deep dive into the current literature on your chosen topic, and identify 3-4 major sub-areas.

For each sub-area, identify the main challenges and choose 2-3 papers that are representative of that sub-area: you *should* include relevant readings that we discussed in class, but they do *not* count towards the 2-3 paper requirement. For each paper, you will summarize and analyze the authors' methods (experimental design, model architecture, and training procedure) and results: you are essentially expected to act as a "mini Discussion Leader" (minus the "field questions" part) for each of these papers, but in a written format (obviously). 

There is no minimum length for the term paper: if you satisfy all of the requirements described above, your paper will be long enough (I'm expecting these to be somewhere in the neighborhood of eight pages). There is also no strict maximum page count. That being said, please limit your paper to a reasonable length: I would really prefer not to have to read fifteen fifty-page papers at the end of the course!

Term papers will be due by March 21, 2025, and should be submitted in ACL format. 
