# _GPR-Protocol_ -> Generative Programmable Response Protocol

## Problem Statement

Current text-based emotion recognition systems are primarily limited by their reliance on **static**, **predefined emotion categories** and **fixed training datasets**, leading to a restricted ability to:

1. comprehensively understand the _nuanced_, _mixed_, and _abstract_ spectrum of human emotions;
2. adapt to _evolving linguistic expressions of sentiment in real-time_;
3. dynamically discover and integrate novel emotional concepts without extensive, manual re-engineering.

This limits their effectiveness in achieving genuinely adaptive and human-aligned emotional intelligence.

## Motivation

WE AREN'T MOTIVETED YET ...

## Objective/Goal

Develop a **Real-Time Continual Learning Emotional AI** capable of dynamically building and maintaining a **universal, multidimensional emotional landscape** from any kind of input/s.

## Approach:

The **JAST emotional AI Framework** is a dynamic, continual-learning approach designed to transcend static, categorical emotion recognition by mapping text onto a continuous, **four-dimensional bipolar emotional space** (**JAST-V Points**). This space is organized around the foundational psychological axes of **Joy/Sadness, Anger/Fear, Surprise/Anticipation, and Trust/Disgust**. To ensure the prototype is viable on resource-constrained hardware like the Raspberry Pi 4B, the system for **Natural Emotion Processing (NEP)** pivots from a heavy Transformer to a lightweight **2-Layer Bi-GRU** neural network, which is then dramatically accelerated for real-time inference using **INT8 Dynamic Quantization**.

The system's intelligence and personalization come from its **Human-in-the-Loop (HITL) Continual Learning** strategy. After initial supervised training to establish a universal emotional map, the model continuously refines its understanding based on your daily feedback. By correcting the model's daily log of JAST-V coordinates, you provide the **Preference Signals** that align the EAI's affective mimicry to your unique expression, a process analogous to **RLHF**. This active refinement, supported by techniques like a replay buffer to combat **Catastrophic Forgetting**, allows the AI to dynamically discover and integrate nuanced emotional concepts specific to your linguistic style.

For more detailed description/information look into [this file](Architectur-v0.1.md).

## Expected outcomes

OTO JANI NA ...

## Major contribution

OTO JANI NA ...

## Team Members and Contributors

1. Srijan Bhattacharyya [![Team Leader](https://img.shields.io/badge/Team%20Leader-ff0000?style=plastic)]()
2. Arijit Ghosh [![Member](https://img.shields.io/badge/Member-ff0000?style=plastic)]()
3. Kushal Biswas [![Member](https://img.shields.io/badge/Member-ff0000?style=plastic)]()
4. Pukar Sharma [![Member](https://img.shields.io/badge/Member-ff0000?style=plastic)]()
5. Jhumki Barman [![External Member](https://img.shields.io/badge/External%20Member-ff0000?style=plastic)]()

## Mentors

1. Dr. Utsa Roy [![Mentor](https://img.shields.io/badge/Mentor-ff0000?style=plastic)]()
2. Dr. Monojit Chattarjee [![External Mentor](https://img.shields.io/badge/External%20Mentor-ff0000?style=plastic)]()

## Bibliography ....

PORE LIKHBO ...
