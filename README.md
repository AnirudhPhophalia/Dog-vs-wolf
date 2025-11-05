# Dog vs Wolf Image Classification 🐕🐺

A deep learning project that uses Convolutional Neural Networks (CNN) to classify images as either dogs or wolves. This project demonstrates the application of computer vision and neural networks to solve a binary image classification problem.

## 📋 Project Overview

This project implements a CNN-based image classifier that can distinguish between images of dogs and wolves with approximately 81% accuracy. The model is built using TensorFlow and Keras, and includes data augmentation techniques to improve model performance.

## 🎯 Features

- **Binary Image Classification**: Accurately classifies images as dogs or wolves
- **Data Augmentation**: Implements image augmentation to improve model generalization
- **CNN Architecture**: Uses a multi-layer convolutional neural network
- **Training Visualization**: Provides plots for training and validation accuracy
- **Google Colab Support**: Can be run directly in Google Colab

## 🗂️ Dataset

The project uses the [Dogs vs Wolves dataset](https://www.kaggle.com/datasets/harishvutukuri/dogs-vs-wolves) from Kaggle, which contains:
- **Training Set**: 1,600 images (80% split)
- **Validation Set**: 400 images (20% split)
- **Image Size**: Resized to 150x150 pixels
- **Classes**: 2 (Dogs and Wolves)

## 🏗️ Model Architecture

The CNN model consists of the following layers:

```
1. Conv2D Layer (32 filters, 3x3 kernel, ReLU activation)
2. MaxPooling2D (2x2 pool size)
3. Conv2D Layer (64 filters, 3x3 kernel, ReLU activation)
4. MaxPooling2D (2x2 pool size)
5. Conv2D Layer (128 filters, 3x3 kernel, ReLU activation)
6. MaxPooling2D (2x2 pool size)
7. Flatten Layer
8. Dense Layer (512 neurons, ReLU activation)
9. Dense Layer (1 neuron, Sigmoid activation)
```

**Model Configuration:**
- **Optimizer**: Adam
- **Loss Function**: Binary Crossentropy
- **Metrics**: Accuracy
- **Training Epochs**: 20

## 🚀 Getting Started

### Prerequisites

```bash
Python >= 3.7
tensorflow
kagglehub
matplotlib
numpy
scikit-learn
Pillow
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/AnirudhPhophalia/Dog-vs-wolf.git
cd Dog-vs-wolf
```

2. Install required dependencies:
```bash
pip install kagglehub tensorflow matplotlib numpy scikit-learn Pillow
```

### Usage

#### Option 1: Google Colab (Recommended)

Click the badge below to open the notebook in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AnirudhPhophalia/Dog-vs-wolf/blob/main/dog_vs_wolf.ipynb)

#### Option 2: Local Jupyter Notebook

1. Start Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `dog_vs_wolf.ipynb` and run all cells sequentially

#### Option 3: Python Script

Run the notebook cells in sequence, which will:
1. Download the dataset from Kaggle
2. Split data into training and validation sets
3. Apply data augmentation
4. Build and compile the CNN model
5. Train the model for 20 epochs
6. Evaluate model performance
7. Display accuracy plots

## 📊 Results

The model achieves the following performance:
- **Test Accuracy**: ~81%
- **Training Duration**: 20 epochs
- **Image Processing**: Data augmentation applied for better generalization

The training process includes visualization of:
- Training accuracy over epochs
- Validation accuracy over epochs
- Training vs validation accuracy comparison

## 🛠️ Technologies Used

- **Python**: Core programming language
- **TensorFlow/Keras**: Deep learning framework
- **KaggleHub**: Dataset downloading
- **NumPy**: Numerical computations
- **Matplotlib**: Data visualization
- **Scikit-learn**: Data splitting utilities
- **Pillow (PIL)**: Image processing

## 📁 Project Structure

```
Dog-vs-wolf/
│
├── dog_vs_wolf.ipynb     # Main Jupyter notebook with complete implementation
└── README.md             # Project documentation
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Future Improvements

- Increase model accuracy through hyperparameter tuning
- Implement transfer learning with pre-trained models (VGG16, ResNet, etc.)
- Add support for multi-class classification (more animal species)
- Create a web interface for image upload and prediction
- Deploy the model as a REST API

## 📄 License

This project is open source and available for educational purposes.

## 👤 Author

**Anirudh Phophalia**
- GitHub: [@AnirudhPhophalia](https://github.com/AnirudhPhophalia)

## 🙏 Acknowledgments

- Dataset provided by [Harish Vutukuri](https://www.kaggle.com/harishvutukuri) on Kaggle
- TensorFlow and Keras documentation
- Google Colab for providing free GPU resources

---

⭐ If you found this project helpful, please consider giving it a star!