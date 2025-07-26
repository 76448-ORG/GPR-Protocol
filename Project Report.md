# Project Name
1. Emotion Recognition and Expression using AI, ML, DL.
2. **GPR-Protocol** -> Generative Programmable Response Protocol
3. ...

## Project idea (Brief Overview)
AKHONO KICHU NEI ...

## Problem Statement 
Current text-based emotion recognition systems are primarily limited by their reliance on **static**, **predefined emotion categories** and **fixed training datasets**, leading to a restricted ability to: 
1. comprehensively understand the _nuanced_, _mixed_, and _abstract_ spectrum of human emotions; 
2. adapt to _evolving linguistic expressions of sentiment in real-time_;
3. dynamically discover and integrate novel emotional concepts without extensive, manual re-engineering.

This limits their effectiveness in achieving genuinely adaptive and human-aligned emotional intelligence.

Develop a **Real-Time Continual Learning Emotional AI** capable of dynamically building and maintaining a **universal, multidimensional emotional landscape** from any kind of input/s.

## Motivation 
WE AREN'T MOTIVETED YET ...

## Objectives/Goals 
To understand and express human emotions from texts using AI, ML and DL.

## Potential Approach 
<details>
  <summary><strong>Approach 1:</strong><br>Built a constantly evolving EAI using Self-Supervised Learning which discovers/plots emotional vector point in a multi-dimensional coordinate space guided by real-time HITL feedback and continual learning techniques.</summary>

### Description:
This approach builds a dynamic **Emotional Artificial Intelligence (EAI)** by representing text as points in a multi-dimensional space via **self-supervised learning**, then continuously refines and discovers emotional categories (from basic to abstract/mixed) through **real-time human-in-the-loop HITL feedback** and continual learning, creating a constant, universal emotional map independent of individual conversations.

### Advantages:
1.  **Dynamic & Adaptive Understanding:** The AI continuously learns and updates its emotional map, adapting to new linguistic nuances, slang, and evolving expressions of emotion without needing complete retraining.
2.  **Discovery of Novel Emotions:** It's not limited to predefined categories. The system can discover and incorporate entirely new, complex, or abstract emotions (like "sarcasm", "nostalgia", "grudge", etc.) as they emerge from interactions and are labeled by human guides.
3.  **Handling of Mixed/Nuanced Emotions:** The multidimensional space naturally represents the blending and subtlety of human feelings, allowing the AI to understand that a text might express a mix of "sadness" and "anger" (e.g., "frustration").
4.  **Reduced Reliance on Massive Labeled Datasets:** While some initial labeling is needed, the continual learning and human-in-the-loop aspects mean it doesn't require a prohibitively large, perfectly labeled dataset for every single emotion from day one. It learns incrementally.
5.  **Improved Robustness & Generalization:** By learning from diverse, real-time "surroundings," the AI becomes more robust to variations in how people express emotions and can generalize its understanding to unseen contexts.
6.  **Human Alignment:** Direct human feedback ensures the AI's emotional understanding aligns with human perception, which is crucial for subjective concepts like feelings.
7.  **Efficiency in Updates:** Continual learning techniques (like PEFT) allow for efficient updates to the model without forgetting prior knowledge, avoiding costly and time-consuming full retraining cycles.
8.  **Constant Universal Map:** The established emotional map remains constant across users, providing a stable and consistent basis for emotional interpretation, while individual conversations use this map for real-time analysis.

### Disadvantages:
1.  **High Human Annotation Cost & Effort:**
    * **Scalability Bottleneck:** Human feedback is indispensable, but acquiring consistent, high-quality labels for complex, nuanced, or abstract emotions at scale is extremely time-consuming and expensive. You can't simply automate this core teaching process.
    * **Subjectivity & Inconsistency:** Human perception of emotions can be subjective and vary between annotators, especially for abstract or mixed feelings. This inconsistency can introduce noise into the training data and make the AI's learning more difficult.
    * **Expertise Required:** For certain complex or domain-specific emotions, you might need highly trained experts, further increasing costs and limiting availability.

2.  **Catastrophic Forgetting Risk (The Continual Learning Challenge):**
    * This is the biggest technical hurdle. Without careful design, as the AI learns new emotions or refines its understanding, it might "forget" previously learned basic or complex emotions, degrading its performance on old data. Preventing this requires sophisticated and computationally intensive techniques.

3.  **Complexity of Model Management:**
    * **Dynamic Updates:** Managing a model that is constantly being updated in real-time is much more complex than static models. Version control, deployment, and ensuring stability become significant engineering challenges.
    * **Debugging Difficulties:** When an issue arises, it's harder to pinpoint whether it's due to new data, a misinterpretation by the human guide, or an issue with the continual learning algorithm itself.

4.  **Interpretability ("Black Box" Problem):**
    * While you'll have a multidimensional graph, truly understanding *why* the AI classifies a specific input as a particular complex emotion (e.g., the precise combination of features in the embedding that trigger "grudge") can be very difficult due to the inherent complexity of deep learning models. This can make debugging and building trust challenging.

5.  **Bias Amplification:**
    * If the initial training data or the human feedback contains biases (e.g., cultural, gendered, or regional biases in emotional expression), the AI will learn and potentially amplify these biases in its "universal" emotional map. Careful monitoring and bias mitigation strategies are crucial.

6.  **Computational Resources:**
    * Training large embedding models, implementing continual learning, and maintaining a real-time system can be computationally very expensive, requiring significant hardware and cloud resources.

7.  **Cold Start Problem for New Emotions:**
    * While it can discover new emotions, when a truly *novel* emotion or expression appears for the first time, the AI will initially be completely unequipped to handle it, requiring explicit human intervention and a sufficient number of examples before it can reliably recognize it on its own.

### Limitations:
1.  **Lack of True Sentience/Feeling:**
    * **No Subjective Experience:** The AI will never *feel* emotions. Its "understanding" is purely computational – it models patterns in language and learns correlations. It cannot replicate the biological and conscious experience of human emotion. This means it can never truly "empathize" in the human sense.

2.  **Reliance on Linguistic Expression:**
    * **Text-Bound:** The AI's emotional understanding is entirely derived from text. It cannot perceive non-verbal cues (facial expressions, tone of voice, body language), which are crucial for full human emotional understanding. This limits its ability to fully grasp context or detect subtle non-linguistic emotional signals.

3.  **Contextual Ambiguity & Nuance Beyond Text:**
    * **Real-World Context:** Emotions are deeply intertwined with real-world situations, shared histories, and cultural backgrounds that may not be fully captured in text alone. The AI might struggle with implicit emotions, sarcasm, or irony if it lacks broader world knowledge or shared cultural context that isn't explicitly stated in the text.
    * **Tacit Knowledge:** Humans understand many things implicitly. The AI's understanding will always be limited by what can be expressed or inferred from the linguistic data it processes and the explicit feedback it receives.

4.  **Bias Inherent in Data & Human Feedback:**
    * **Perpetuation of Societal Biases:** If the language data it learns from, or the human annotators providing feedback, reflect societal biases (e.g., gender stereotypes in emotional expression, cultural differences in emotional labeling), the AI will inevitably learn and potentially perpetuate these biases. Achieving a truly "universal" and unbiased emotional map is an ongoing and difficult challenge.

5.  **Interpretability Challenges (Understanding "Why"):**
    * While you plot points in a multidimensional graph, comprehending *why* a specific complex embedding lands in a particular emotional cluster can remain a "black box" problem. The AI can tell you *what* emotion it perceives, but not necessarily the intricate reasoning or specific linguistic features that led to that perception, limiting deep human insight into its emotional "logic."

6.  **Scalability of "New Emotion" Discovery:**
    * While it can discover new emotions, the efficiency of this discovery relies heavily on sufficient, consistent human feedback. If a new emotional expression is very rare or highly ambiguous, it might take a long time and many feedback cycles for the AI to reliably form a new cluster and understand it. The rate of human labeling can be a bottleneck for truly novel emotion discovery.

</details>

<details>
  <summary><strong>Approach 2:</strong><br>Built a context aware classification system using BERT and trained model.</summary>

### Description:
### Advantages:
### Disadvantages:
### Limitations:
</details>

## Expected outcomes and Major contribution
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
