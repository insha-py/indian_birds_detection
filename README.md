
# Indian Birds Detection System

## Overview
This project focuses on building an image classification model to detect and classify Indian bird species using deep learning techniques. The model was trained on an augmented dataset of 25 bird categories and tested using two different architectures: **ResNet50** and **EfficientNet**. The results showed that EfficientNet outperformed ResNet50, achieving an accuracy of **80%**, compared to **70%** with ResNet50.

## Dataset
- The dataset consists of images of 25 Indian bird species.
- Data augmentation techniques were applied to improve model robustness.
- Each image was preprocessed and resized before feeding into the neural networks.

## Model Architectures
### **ResNet50**
- A deep residual network with 50 layers.
- Achieved **70% accuracy** on the test set.

### **EfficientNet**
- A more efficient convolutional neural network with optimized scaling.
- Achieved **80% accuracy**, outperforming ResNet50.

## Training Details
- **Loss Function**: Cross-entropy loss
- **Optimizer**: Adam
- **Learning Rate**: Tuned using experimentation
- **Batch Size**: Set optimally based on memory constraints
- **Epochs**: Determined through early stopping to avoid overfitting
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score

## Results & Observations
| Model       | Accuracy |
|------------|----------|
| ResNet50   | 70%      |
| EfficientNet | 80%      |

- EfficientNet performed better due to its optimized architecture for feature extraction.
- Data augmentation played a crucial role in improving the model's generalization.
- Further improvements can be made by fine-tuning hyperparameters and using a larger dataset.

## Future Improvements
- Implement **bounding box detection** to enable object localization.
- Experiment with **transformer-based models** like Vision Transformers (ViTs).
- Incorporate **active learning** to refine the dataset with user feedback.
- Deploy as a web or mobile application for real-world use.

## How to Use
### **1. Install Dependencies**
```
pip install tensorflow numpy pandas matplotlib opencv-python
```

### **2. Run the Model**
```python
python train.py --model efficientnet --epochs 30
```

### **3. Predict on New Images**
```python
python predict.py --image path/to/image.jpg
```

## Acknowledgments
- Inspired by the need for bird conservation and species identification in India.
- Thanks to the open-source datasets and deep learning frameworks used in this project.

## License
This project is open-source and available under the MIT License.

