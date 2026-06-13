# Plant Disease Detection using CNN
------------------------------------------------------------------------------

It is deep learning project that classifies plant leaf images into different disease categories using a Convolutional Neural Network (CNN) trained on the PlantVillage dataset.

**🚀 Features**
------------------------------------------------------------------------------

🌱 Image Classification Model — Predicts plant diseases from leaf images

🧠 Deep CNN Architecture — Multiple convolution layers with Batch Normalization

📊 Data Augmentation — Rotation, zoom, and flipping to improve generalization

⚡ Global Average Pooling — Reduces overfitting and improves performance

📉 Early Stopping — Stops training when model stops improving

📈 Performance Evaluation — Accuracy, precision, recall, F1-score

🧠 Model Architecture
------------------------------------------------------------------------------
```bash
Input: 128 × 128 × 3 image
        ↓
Conv2D + Batch Normalization + MaxPooling (4 blocks)
        ↓
Global Average Pooling
        ↓
Dense Layer (256 neurons, ReLU activation)
        ↓
Dropout Layer (0.5)
        ↓
Output Layer (Softmax for multi-class classification)
```
**Training Setup**
------------------------------------------------------------------------------

```bash
- Loss Function: Categorical Crossentropy
- Optimizer: Adam (learning rate = 0.0001)
- Metric: Accuracy
- Early Stopping (patience = 3)
```
⚙️ Preprocessing
------------------------------------------------------------------------------

Image resizing to 128×128

Normalization (rescale 1./255)

Data augmentation:

- Rotation

- Zoom

- Horizontal flip

📊 Evaluation Metrics
------------------------------------------------------------------------------

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report (per class performance)
