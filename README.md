# AI Group Research Project: Chatbot Arena Human Preference Predictions

Welcome to the GitHub repository for the **Chatbot Arena Human Preference Predictions** project! This project is focused on building a machine learning model that can predict human preferences between responses from two Large Language Models (LLMs). The project is part of the **LMSYS - Chatbot Arena Human Preference Predictions** competition.

## 🧠 **Project Brief**

The primary goal of this project is to develop a model that accurately predicts which LLM-generated response a human judge will prefer. We will explore different machine learning techniques, including **supervised learning** and **reinforcement learning from human feedback (RLHF)**. Additionally, we aim to address and mitigate common biases like verbosity and position bias in the responses.

## 📅 **Project TODO**

Here is a brief list of the tasks that need to be completed to implement this project:

1. **Data Collection and Preprocessing:**
   - [ ] Load the competition dataset (55K rows of conversational data).
   - [ ] Implement data augmentation techniques (synonym replacement, paraphrasing, position shuffling).
   - [ ] Ensure proper data split between training and testing sets.

2. **Feature Engineering:**
   - [ ] Extract contextual embeddings using **BERT** or **RoBERTa**.
   - [ ] Create additional features, such as response length, sentiment score, and word overlap.

3. **Model Training (Supervised Learning):**
   - [ ] Implement different classifiers: Random Forest, Gradient Boosting, and Transformer-based models.
   - [ ] Train models using supervised learning to predict the preferred response.

4. **Bias Mitigation:**
   - [ ] Implement techniques to reduce verbosity, position, and self-enhancement biases.
   - [ ] Evaluate the effect of bias mitigation on model performance.

5. **Reinforcement Learning from Human Feedback (RLHF):**
   - [ ] Fine-tune the model using **Proximal Policy Optimization (PPO)** for RLHF.
   - [ ] Train the reward model to optimize alignment with human preferences.

6. **Evaluation:**
   - [ ] Evaluate the model's performance using **log loss** as the primary metric.
   - [ ] Track bias metrics to ensure fair prediction of human preferences.
   - [ ] Conduct ablation studies to identify the most effective methods.

7. **Final Testing and Results:**
   - [ ] Test the model on the competition dataset.
   - [ ] Store results and share visualizations of key metrics.

## 📝 **Next Steps**

- Set up a Python environment with all necessary dependencies.
- Begin with data collection and preprocessing.
- Establish the baseline models with supervised learning techniques.
- Iterate and refine the approach using RLHF and bias mitigation.

---

Stay tuned for updates as we progress through the project!
