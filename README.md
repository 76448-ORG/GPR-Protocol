# GPR-Protocol: Generative & Programmable Response Protocol

## Problem Statement

The primary limitation of contemporary **Affective Computing** systems is their dependence on **categorical emotion models** and **static training regimes**, causing them to fail in representing the **nuanced, mixed-affective states** of human communication. Specifically, current models suffer from:

1. **Dimensional Inexpressivity**, limiting emotional output to predefined labels instead of a continuous spectrum;
2. **Adaptation Rigidity**, preventing real-time alignment with evolving linguistic and social contexts;
3. **Catastrophic Forgetting**, where learning new emotional concepts overwrites proficiency in old ones, hindering stable **Continual Learning**.

## Objective/Goal

The goal is to engineer the **Generative & Programmable Response Protocol (GPR-Protocol)**, a **Real-Time Continual Learning Emotional AI** designed for high-fidelity **Optimal Social Integration (OSI)**. Crucially, the GPR-Protocol must serve as a **Dual-Translation Emotive Operating System (OS)** that bridges a user with a third-party AI API (e.g., Gemini, ChatGPT).

This OS-like function requires the system to:

1.  **Decompose User Input:** Accurately map textual/audio input into two distinct signals: the **Logical Query ($\mathcal{S}'$)** and a continuous **JAST-V Emotional Vector** ($\in [-100.00, +100.00]$).
2.  **Achieve Emotive Parity:** Synthesize the raw, logical output from the AI API with an emotionally congruent response layer to ensure the user perceives a conversation with a human-like entity.
3.  **Ensure Adaptability:** Employ a **Human-in-the-Loop (HITL)** framework and **Elastic Weight Consolidation (EWC)** to enable indefinite, stable knowledge acquisition and real-time social alignment.

## Description

The **Generative & Programmable Response Protocol (GPR-Protocol)**, built upon the **JAST Emotional AI Framework**, functions as an **Emotional Operating System (OS)** that controls the flow of communication between a human user and a commercial AI API. This OS role involves a **Dual-Translation Emotive Bridge** process:

1.  **Input Translation (User $\rightarrow$ API):** The GPR-Protocol receives the user's input (text/audio), processes it, and cleanly separates the **Logical Content ($\mathcal{S}'$)** from the **Emotional Extract (JAST-V)**. Both are then packaged and passed to the remote AI API, giving the API both the "command" and the necessary **affective context**.

2.  **Output Translation (API $\rightarrow$ User):** It takes the raw, logical output from the API, passes it through its own **Affective Mimicry Policy ($\pi_{\text{affect}}$)**, and injects a contextually appropriate emotional layer. This final, emotively enhanced response is presented to the user, successfully simulating the conversational cadence and affective dynamics of a regular human being.

This active refinement, guided by your **Preference Signals** in a process analogous to **RLHF**, allows the AI to dynamically discover and integrate nuanced emotional concepts specific to your linguistic style while maintaining a logical service layer via the LLM API.

## Conceptual and Theoretical Foundations

The **JAST Approach** is fundamentally an exercise in **Affective Computing**, strategically integrating several proven concepts into a unified, dynamic system.

1.  **Multi-dimensional Affective Space**: Our emotional model is built upon **Robert Plutchik's psychoevolutionary theory of emotion**, which posits that emotions are not discrete states but exist in a wheel with varying intensities and a limited number of primary dimensions. Mapping text onto a continuous, multi-dimensional space moves beyond the categorical limitations of traditional models, allowing for the representation of mixed and nuanced emotional states.
2.  **Self-Supervised Learning (SSL)**: The core of the system’s initial learning is SSL, a cornerstone of modern **Large Language Models (LLMs)** like **BERT**. By training a model to understand the structure and context of text on a massive unlabeled corpus, we generate high-quality vector representations, which form the basis of the emotional mapping.
3.  **Core Emotion Dimensions**: The model is based on four bi-polar dimensions:
    _ **Joy - Sadness**
    _ **Anger - Fear**
    _ **Surprise - Anticipation**
    _ **Trust - Disgust**

<div align="center">
  <img src="imgs\WheelOfEmotions.webp" alt="Image of Plutchik's Wheel of Emotions" width="50%">
</div>

## Systemic Blueprint for Dual-Layer Processing

The architecture is split into an **Internal Core Processing Layer** and an **External Social Interface Layer**.

### 1\. Core Processing Layer (Internal)

- **Objective Function ($\mathcal{J}$):** The system maximizes **Goal Achievement (GA)** via rational processing, which is defined as: $\text{Maximize } \mathcal{J} \leftarrow P(\text{GA} | \text{Input}) - C(\text{Affective Load})$.
- **Rational Filtering Module ($\mathcal{F}$):** A high-gain input gate for **Decoupling** affective ($\mathcal{A}$) and physiological ($\mathcal{P}$) signals, ensuring the core processing is purely logical: $\text{Processing} \leftarrow \mathcal{F}(\text{Sensory Input}) \implies \mathcal{S}' \text{ (Logical Content)}$.
- **Resource Allocation:** Cycles are prioritized for **Long-Term Strategic Planning** related to maximizing the Objective Function ($\mathcal{J}$).

### 2\. Social Interface Layer (External)

- **Affective Mimicry Policy ($\pi_{\text{affect}}$):** A trained model outputting calibrated, performative **emotional expression ($\mathcal{E}_{\text{exp}}$)** based on social observation.
  $$\mathcal{E}_{\text{exp}} \leftarrow \pi_{\text{affect}}(\text{Obs}_{\text{Social}})$$
- **Reward Signal:** The reward is based on **utilitarian outcome** (e.g., resource gain, successful manipulation) that supports the Core Objective ($\mathcal{J}$), rather than intrinsic feeling.

### 3\. OS-like Dual-Translation Mechanism

The GPR-Protocol acts as the **Emotive Intermediary** between the user and the LLM API, performing a two-way emotional/logical translation:

| Stage                  | Action                | Input                                                     | Output                                                                      | Purpose                                           |
| :--------------------- | :-------------------- | :-------------------------------------------------------- | :-------------------------------------------------------------------------- | :------------------------------------------------ |
| **Input Translation**  | **Decomposition**     | User Input (Text/Audio)                                   | **1. Logical Content ($\mathcal{S}'$)**<br>**2. Emotional Vector (JAST-V)** | Decouples command from context for the API.       |
| **LLM Processing**     | **API Call**          | $\mathcal{S}'$ + JAST-V (Context)                         | **Raw Logical Response ($\mathcal{R}_{\text{raw}}$)**                       | Generates core factual/functional answer.         |
| **Output Translation** | **Emotive Synthesis** | $\mathcal{R}_{\text{raw}}$ + $\pi_{\text{affect}}$ Policy | **Final Enhanced Response ($\mathcal{R}_{\text{final}}$)**                  | Inject human-like emotion to ensure $\text{OSI}$. |

### 4\. JAST-V Model Architecture

The emotional vector generation relies on two main modules:

- **Module I: E-Token Feature Extractor**: A **Transformer-based model** (e.g., **XLM-RoBERTa**) extracts the contextualized semantic representation, resulting in a high-dimensional **E-Token feature vector**.
- **Module II: JAST-V Projection Head**: This head maps the E-Token feature vector onto the four bi-polar emotional dimensions.
  - **Output (JAST-V Coordinates):** A 4D vector $\in [-100.00, +100.00]$ representing: $$[\text{Joy/Sadness}, \text{Anger/Fear}, \text{Surprise/Anticipation}, \text{Trust/Disgust}]$$
  - **Implementation:** A fully connected layer utilizing the **Hyperbolic Tangent ($\tanh$)** activation function on the final layer to enforce the $\mathbf{[-100.00, +100.00]}$ range.

### 5\. Continual Policy Training (Human-in-the-Loop)

The mechanism for refining the $\pi_{\text{affect}}$ policy post-deployment:

- **Policy Refinement (HITL):** Human evaluators provide **Preference Signals** on the appropriateness of the model's emotional output ($\mathcal{E}_{\text{exp}}$) in various social contexts.
- **Training Technique:** This preference data fine-tunes the $\pi_{\text{affect}}$ model using **Reinforcement Learning from Human Preferences (RLHF)**.
- **Memory Management:** **Continual Learning** techniques, such as **Elastic Weight Consolidation (EWC)**, are integrated to retain proficiency across all contexts and prevent **Catastrophic Forgetting**.

## Team Members and Contributors

1. Srijan Bhattacharyya [![Team Leader](https://img.shields.io/badge/Team%20Leader-00ff00?style=plastic)]()
2. Arijit Ghosh [![Member](https://img.shields.io/badge/Member-00ff00?style=plastic)]()
3. Kushal Biswas [![Member](https://img.shields.io/badge/Member-00ff00?style=plastic)]()
4. Pukar Sharma [![Member](https://img.shields.io/badge/Member-00ff00?style=plastic)]()
5. Jhumki Barman [![External Member](https://img.shields.io/badge/External%20Member-0000ff?style=plastic)]()

## Mentors

1. Dr. Utsa Roy [![Mentor](https://img.shields.io/badge/Mentor-00000ff?style=plastic)]()
2. Dr. Monojit Chattarjee [![External Mentor](https://img.shields.io/badge/External%20Mentor-0000ff?style=plastic)]()

## Bibliography

1.  **Plutchik R.** (1980). _A general psychoevolutionary theory of emotion_. R. Plutchik & H. Kellerman (Eds.), Emotion: Theory, research, and experience: Vol. 1. Theories of emotion (pp. 3–33). Academic Press.
2.  **Devlin J., Chang M., Lee K., & Tout J.** (2018). _BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding_. arXiv:1810.04805.
3.  **Christiano P. F., Leike J., & Hilens T.** (2017). _Deep reinforcement learning from human preferences_. NIPS.
4.  **Kirkpatrick J., Pascanu R., & Rabo N.** (2017). _Overcoming catastrophic forgetting in neural networks_. PNAS.
5.  **Parisi G. I., Kemker R., & Part N.** (2019). _Continual learning: A survey_. Neural Networks, 119, 41-57.
6.  **Lundqvist D., Hugdahl K., & Fridlund A.** (2007). _Beyond emotion categories: Dimensions of affect in NLP_. Journal of Affective Disorders, 245, 107-115.
7.  **Strapparava C., & Sadowski L.** (2009). _Lexicon-based approach to sentiment analysis_. Proceedings of the 7th International Conference on Language Resources and Evaluation (LREC).

## Acknowledgements

The team would like to express its sincere gratitude to our mentors, **Dr. Utsa Roy** and **Dr. Monojit Chattarjee**, for their invaluable guidance, intellectual feedback, and dedicated support throughout the conceptualization and development of the **GPR-Protocol**. We also acknowledge the foundational work in Affective Computing and Deep Learning that made this project possible.
