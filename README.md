# LLM Response Preference Prediction System

A machine learning system for predicting human preferences between LLM-generated responses, developed as part of the LMSYS Chatbot Arena Competition.

## Overview

This project develops advanced ML models to predict which LLM-generated response a human evaluator would prefer. We leverage supervised learning and RLHF techniques while addressing common biases in language model outputs.

### Key Features

- Processing of 55K+ conversational pairs
- BERT/RoBERTa-based contextual embeddings
- Bias mitigation for position and verbosity
- RLHF implementation using PPO
- Comprehensive evaluation framework

## Technical Implementation

### Data Pipeline
- Large-scale dataset processing (55K conversations)
- Advanced augmentation techniques:
  - Synonym replacement
  - Contextual paraphrasing
  - Position-aware shuffling
- Robust train/test splitting

### Model Architecture
- Feature Engineering:
  - BERT/RoBERTa embeddings extraction
  - Multi-modal feature integration
  - Response metrics computation
- Training Methods:
  - Ensemble of classical ML (Random Forest, GBM)
  - Transformer-based neural networks
  - PPO-based RLHF fine-tuning

### Bias Mitigation
- Position bias reduction
- Verbosity normalization
- Self-enhancement correction
- Performance impact analysis

## Evaluation Framework

- Primary Metric: Log Loss
- Bias Assessment Metrics
- Ablation Studies
- Real-time Performance Tracking

## Technical Requirements

- Python 3.8+
- Key Libraries:
  - PyTorch
  - Transformers
  - scikit-learn
  - Ray
  - Weights & Biases

## Development Roadmap

1. Environment Setup & Data Pipeline
2. Baseline Model Development
3. RLHF Integration
4. Bias Mitigation Implementation
5. Evaluation & Optimization
6. Competition Submission

## Getting Started

```bash
# Clone repository
git clone https://github.com/anudeepadi/Chatbot-Arena-Human-Preference-Predictions.git

# Install dependencies
pip install -r requirements.txt

# Run baseline training
python src/train.py --config configs/baseline.yaml

# Execute RLHF fine-tuning
python src/rlhf_train.py --model baseline --epochs 10
```

## Project Status

Currently implementing core model architecture and data processing pipeline. Contributions welcome for bias mitigation strategies and RLHF implementation.
