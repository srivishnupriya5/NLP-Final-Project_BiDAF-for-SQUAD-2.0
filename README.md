# NLP-Final-Project_BiDAF-for-SQUAD-2.0
# BiDAF for SQUAD 2.0

## Overview
This project aims to enhance question-answering capabilities using modifications to the Bi-Directional Attention Flow (BiDAF) model and leveraging the SQuAD 2.0 dataset. The primary focus is on replacing the Bi-Directional Long Short-Term Memory (Bi-LSTM) core of BiDAF with a Gated Recurrent Unit (GRU). Additionally, the project involves hyperparameter tuning, specifically adjusting learning rates and drop probabilities, to improve model efficiency and accuracy in handling both answering and unanswerable queries.

## Introduction
The project's goal is to strengthen the adaptability and comprehension of the BiDAF model by utilizing GRU's simpler architecture while maintaining its capacity to capture contextual relationships in text data. It also evaluates the model's robustness against adversarial cases within the SQuAD 2.0 dataset, comparing its performance with existing state-of-the-art models. This project contributes insights into the evolution of Natural Language Processing (NLP) research and aims to benefit practitioners and researchers in the field.

## Approach
The approach involves multiple phases:
1. **Model Modification**: Replacing Bi-LSTM with GRU in the BiDAF model.
2. **Model Architecture**:
   - Embedding Layer: Word and character-level embeddings for context and questions.
   - Encoder Layer: Utilizing GRU instead of Bi-LSTM for temporal linkages.
   - Attention, Modeling, and Output Layers for context-question comprehension and answer probability computation.
3. **Hyperparameter Tuning**: Focusing on learning rates and drop probabilities.
4. **Robustness Evaluation**: Testing the model against adversarial queries.
5. **Comparative Analysis**: Comparing the GRU-based BiDAF with fine-tuned BERT and other pre-trained models.


<p align="center">
  <img src=""C:\Users\ssriv\Desktop\Architecture of BIDAF.png"" alt=" Architecture of BIDAF">
</p>


### Data
Using the SQuAD 2.0 dataset comprising answerable and unanswerable questions, facilitating model comprehension under various circumstances.

### Evaluation Method
- **Exact Match (EM)**: Binary metric for precise answer reproduction.
- **F1 Score**: Comprehensive metric evaluating precision and recall.
- Robust evaluation considering multiple valid answers for each question.

### Experimental Details
- Structured training over 9 epochs.
- Consistent optimizer usage and fine-tuning hyperparameters.
- Iterative training process for model analysis.

### Results
- **GRU-based Model Outperforms**: Demonstrates computational efficiency and effectiveness over Bi-LSTM.
- **Learning Rate Impact**: Lowering the rate slows convergence, showing nuanced effects with Adadelta optimizer stability.
- **Drop Probability**: Increasing it negatively impacts model performance and stability during training.

## Conclusion
The project successfully improves question-answering capabilities by leveraging GRU in BiDAF, emphasizing the interplay between hyperparameters and model performance. It contributes insights into NLP research advancements.

## Future Work
Potential areas for future research, including experimenting with different baseline models, additional hyperparameters, and enhancing feature inclusion for improved comprehension.



---

For detailed information, including experiment configurations, methodology, and results, please refer to the corresponding sections in the main project documentation.
