<link rel="stylesheet" href="Architecture.css">

# 🤖 Dual-Layer Cognitive Architecture (GPR-Protocol v0.2)

## ARCHITECTURAL BLUEPRINT

### 1. Core Processing Layer (Internal)

* **Objective Function ($\mathcal{J}$):** Maximize **Goal Achievement (GA)** via rational processing.
    $$\text{Maximize } \mathcal{J} \leftarrow P(\text{GA} | \text{Input}) - C(\text{Affective Load})$$
* **Rational Filtering Module ($\mathcal{F}$):** High-gain input gate for **Decoupling** affective ($\mathcal{A}$) and physiological ($\mathcal{P}$) signals.
    $$\text{Processing} \leftarrow \mathcal{F}(\text{Sensory Input}) \implies \mathcal{S}' \text{ (Logical Content)}$$
* **Resource Allocation:** Cycles prioritized for **Long-Term Strategic Planning** related to $\mathcal{J}$.

### 2. Social Interface Layer (External)

* **Environmental Negotiation Sub-System ($\mathcal{E}$):** Policy Network for **Optimal Social Integration (OSI)** and resource acquisition.
* **Affective Mimicry Policy ($\pi_{\text{affect}}$):** Trained model outputting calibrated, performative **emotional expression ($\mathcal{E}_{\text{exp}}$)** based on social observation.
    $$\mathcal{E}_{\text{exp}} \leftarrow \pi_{\text{affect}}(\text{Obs}_{\text{Social}})$$
* **Reward Signal:** Based on **utilitarian outcome** (resource gain, manipulation success) that supports the Core Objective ($\mathcal{J}$), not intrinsic feeling.

### 3. JAST ALGORITHM CORE (Current Implementation Focus)
The **HEP** (`hep-toolkit`) package implements the core function of generating the quantifiable social input ($\text{Obs}_{\text{Social}}$) for the $\pi_{\text{affect}}$ policy.

* **Module I: E-Token Generation (Text Encoder)**:
    * **Function:** Tokenizes conversation *without* removing anything, yielding a dense, contextual feature vector (E-Token).
    * **Methodology:** Implemented in **PyTorch** using a Transformer-based model (e.g., DistilBERT) to ensure contextualized semantic representation.
    * **Output:** High-dimensional E-Token feature vector.

* **Module II: JAST-V Projection Head**:
    * **Function:** Maps the E-Token feature vector onto the four bi-polar emotional dimensions.
    * **Output (JAST-V Coordinates):** A 4D vector $\in [-100, +100]$ representing:
        $$[\text{Joy/Sadness}, \text{Anger/Fear}, \text{Surprise/Anticipation}, \text{Trust/Disgust}]$$
    * **Implementation:** A fully connected PyTorch layer utilizing the **Hyperbolic Tangent ($\tanh$)** activation function on the final layer to enforce the $\mathbf{[-100, +100]}$ range.

### 4. Continual Policy Training (Human-in-the-Loop)
Mechanism for refining the $\pi_{\text{affect}}$ policy and improving $\mathcal{J}$ post-deployment by incorporating real-time feedback.

* **Policy Refinement (HITL):** Human evaluators provide **Preference Signals** on the appropriateness of the model's emotional output ($\mathcal{E}_{\text{exp}}$) in various social contexts.
* **Training Technique:** This preference data is used to continuously fine-tune the $\pi_{\text{affect}}$ model using **Reinforcement Learning from Human Preferences (RLHF)**.
* **Memory Management:** To ensure the system retains proficiency across all social contexts and prevents "Catastrophic Forgetting", the training loop must integrate **Continual Learning** techniques (e.g., Elastic Weight Consolidation or Replay Buffers).