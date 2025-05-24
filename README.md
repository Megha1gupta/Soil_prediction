# Soil_prediction

1. Project Objective
The primary objective of this project was to accurately predict soil types or properties using computer vision, leveraging images as input data. This capability can be crucial for applications in agriculture, environmental monitoring, and geological surveys, enabling more efficient and informed decision-making.

2. Methodology
The project employed a robust deep learning approach, integrating pretrained models and an ensemble voting strategy to enhance prediction accuracy and reliability.

Base Models: Two variants of the EfficientNet architecture, EfficientNetB0 and EfficientNetB1, were selected as the foundational pretrained models. These models are known for their efficiency and strong performance across various image recognition tasks.

Instance Generation: Four distinct instances of these models were generated. This involved training each model variant (or multiple instances of the same variant) on the dataset.

Loss Function: To address potential class imbalance within the soil dataset, weighted cross-entropy was utilized as the loss function during model training. This weighting mechanism ensures that the models give appropriate attention to minority classes, preventing bias towards dominant soil types.

Ensemble Voting: To consolidate the predictions from the multiple model instances and improve overall generalization, an ensemble voting mechanism was implemented. In this approach, the final prediction for a given soil image was determined by aggregating the individual predictions from the four trained model instances (e.g., majority voting or weighted voting).

3. Key Result
The ensemble voting strategy proved highly effective, leading to a significant improvement in predictive performance. The project achieved an F1-score of 0.96, indicating excellent balance between precision and recall in soil prediction. This high F1-score demonstrates the model's strong ability to correctly identify various soil types while minimizing both false positives and false negatives.

4. Conclusion
The successful implementation of pretrained EfficientNet models, combined with weighted cross-entropy and an ensemble voting approach, resulted in a highly accurate soil prediction system. The achieved F1-score of 0.96 validates the effectiveness of the chosen methodology for this computer vision task

5. Run instructions
Run jupyter notebook in sequence.