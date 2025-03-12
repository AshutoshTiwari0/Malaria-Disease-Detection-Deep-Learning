# CNN vs. VGG19 Image Classification

## 📌 Overview
This project compares a simple Convolutional Neural Network (CNN) and a pre-trained VGG19 model for image classification. It evaluates the performance of both architectures on a dataset using data augmentation.

## 🛠️ Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib

## 📂 Dataset
- The dataset consists of multiple image classes stored in `Dataset/Train` (for training) and `Dataset/Test` (for validation).
- Images are resized to **224x224x3** for compatibility with VGG19.

## 🔧 Model Architectures

### 1️⃣ **CNN Model**
- Three convolutional layers with ReLU activation.
- MaxPooling after each convolutional layer.
- Fully connected dense layers with softmax activation for classification.

### 2️⃣ **VGG19 Model**
- Uses a pre-trained **VGG19** model (with ImageNet weights).
- The last few layers are replaced with a custom classifier.
- Flattening and dense layers for final predictions.

## 📈 Data Augmentation
- **Rescaling:** Normalized pixel values (1/255)
- **Shear & Zoom Range:** Random distortions and zoom
- **Horizontal Flip:** Enhances variation in training samples

## 🔬 Performance Metrics
| Model  | Train Accuracy | Validation Accuracy | Train Loss | Validation Loss |
|--------|---------------|---------------------|------------|-----------------|
| **CNN** | 83.02% | 46.27% | 0.41 | 0.86 |
| **VGG19** | 87.33% | 77.61% | 0.28 | 0.40 |

## 📊 Visualization
The project includes loss and accuracy plots for both CNN and VGG19 models to illustrate their performance over training epochs.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/AshutoshTiwari0/Malaria-Disease-Detection-Deep-Learning.git
   ```
2. Run Jupyter File
3. View results:
   - Accuracy & loss plots are inside notebook.

## 📌 Conclusion
- **VGG19** outperformed the simple **CNN** in both accuracy and loss.
- Data augmentation improved model generalization.
- The project provides insights into leveraging pre-trained models for better classification.

---
Feel free to contribute or experiment with different architectures! 🚀

