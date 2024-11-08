# Ovarian-Cancer-Subtypes-with-Enhanced-Pre-trained-Models-Using-Differential-Attention
Efficient ovarian cancer subtype classification using pre-trained models with differential attention mechanisms for enhanced precision.


This project focuses on the classification of ovarian cancer subtypes using deep learning models, specifically leveraging pre-trained neural networks enhanced by differential attention mechanisms. Ovarian cancer, known for its heterogeneity, consists of various subtypes such as high-grade serous carcinoma (HGSC), low-grade serous carcinoma (LGSC), endometrioid carcinoma (EC), clear cell carcinoma (CC), and mucinous carcinoma (MC), each with unique clinical and molecular features that demand distinct therapeutic strategies. Effective and precise classification of these subtypes is essential for accurate diagnosis and personalized treatment.

### Project Highlights:
1. **Dataset and Data Preprocessing**:
   - Utilizes a comprehensive ovarian cancer dataset with images categorized into the five subtypes.
   - Employs data augmentation techniques such as rotation, flipping, and scaling to address dataset imbalances and improve model robustness.
   - Resamples data to ensure balanced class distribution using techniques like RandomOverSampler to prevent bias toward majority classes.

2. **Model Architecture**:
   - Builds on state-of-the-art pre-trained models like InceptionV3, Xception, and MobileNet, which are adapted for the classification task.
   - Freezes the base layers of these models to retain pre-trained knowledge, while adding custom top layers tailored to cancer subtype classification.

3. **Differential Attention Mechanism**:
   - Integrates a differential attention layer within the model architecture to enhance feature extraction capabilities. This attention mechanism dynamically focuses on relevant image features, helping distinguish between subtle patterns specific to each subtype.
   - Utilizes a selective attention mechanism that highlights distinguishing features by filtering out noise and emphasizing high-impact regions, critical for accurately differentiating similar subtypes.

4. **Training and Validation**:
   - The model training process incorporates various optimizations like early stopping and learning rate adjustments to prevent overfitting and improve generalization.
   - Divides the dataset into training, validation, and testing subsets using stratified sampling to maintain proportional representation of each subtype.

5. **Evaluation Metrics**:
   - Evaluates model performance based on precision, recall, and F1-score, specific to each subtype. The use of confusion matrices and classification reports helps in identifying any misclassification patterns.
   - Compares model performance across InceptionV3, Xception, and MobileNet to identify the most accurate architecture for ovarian cancer subtype classification, with differential attention acting as a consistent performance booster.

6. **Visualization**:
   - Provides visual interpretations of the model's attention focus through heatmaps and activation maps, helping researchers understand the model's decision-making process.
   - Includes detailed plots of accuracy, loss, and evaluation metrics over each epoch, aiding in assessing model convergence and consistency.

### Potential Impact:
This project offers a powerful tool for pathologists and oncologists to improve diagnostic precision in ovarian cancer. By accurately classifying cancer subtypes, it facilitates more personalized treatment planning, potentially improving patient outcomes.
