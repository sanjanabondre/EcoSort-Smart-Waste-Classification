# ♻️ EcoSort – Smart Waste Classification Using MobileNetV2

EcoSort is an image-based waste classification system that uses **MobileNetV2 and Transfer Learning** to classify waste images into six categories. It provides a simple, interactive web interface to help users understand waste classification and responsible disposal.

## 🌱 Project Overview

Waste segregation is an important step toward effective recycling and environmental sustainability. EcoSort aims to make waste classification easier by using deep learning to predict the category of a waste image and provide a basic disposal recommendation.

## ✨ Features

- 🖼️ **Image Classification:** Upload a waste image to predict its category.
- 🧠 **Deep Learning:** Uses MobileNetV2 with transfer learning.
- ♻️ **Six Waste Categories:** Cardboard, Glass, Metal, Paper, Plastic, and Trash.
- 📊 **Confidence Scores:** Displays the model's predicted class and confidence.
- 🌿 **Disposal Guidance:** Provides a basic disposal tip for the predicted category.
- 💻 **Interactive Interface:** Built using Gradio with a nature-inspired design.

## 🗂️ Waste Categories

The model classifies images into the following categories:

1. Cardboard
2. Glass
3. Metal
4. Paper
5. Plastic
6. Trash

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Deep Learning Framework:** TensorFlow / Keras
- **Pre-trained Model:** MobileNetV2
- **Technique:** Transfer Learning and Fine-Tuning
- **Image Processing:** Pillow and NumPy
- **User Interface:** Gradio
- **Development Environment:** Google Colab
- **Dataset:** TrashNet dataset

## 📚 Dataset

The project uses the TrashNet dataset, which contains images of waste materials organized into six categories.

The dataset used in this project contains **2,527 images**:

| Category | Number of Images |
|---|---:|
| Cardboard | 403 |
| Glass | 501 |
| Metal | 410 |
| Paper | 594 |
| Plastic | 482 |
| Trash | 137 |
| **Total** | **2,527** |

The images were divided into training, validation, and testing sets using a 70:15:15 split.

- Training: 1,766 images
- Validation: 377 images
- Testing: 384 images

Dataset source: [TrashNet Dataset on Kaggle](https://www.kaggle.com/datasets/feyzazkefe/trashnet)

## 🧠 Model Architecture

EcoSort uses MobileNetV2, a lightweight convolutional neural network originally trained on ImageNet.

The model was adapted for six-class waste classification using transfer learning.

**Workflow:**

1. Load and preprocess waste images.
2. Resize images to 224 × 224 pixels.
3. Load the pre-trained MobileNetV2 model.
4. Freeze the base model and train a new classification head.
5. Fine-tune selected layers using a low learning rate.
6. Evaluate the model on the test dataset.
7. Predict the waste category for uploaded images.

The classification head includes Global Average Pooling, Dropout, and a Softmax output layer.

## 📈 Model Performance

After fine-tuning, the model achieved approximately **83.07% test accuracy** on the held-out test dataset.

| Evaluation Stage | Test Accuracy |
|---|---:|
| Initial training | Approximately 82% |
| After fine-tuning | 83.07% |

Fine-tuning improved the test accuracy by approximately 1.07 percentage points based on the recorded comparison.

*Note: Results may vary with different data splits, training settings, and environments.*

## 🖥️ User Interface

The Gradio interface allows users to upload a waste image and view:

- Predicted waste category
- Prediction confidence
- Class scores
- Suggested disposal guidance

Add screenshots of your working application here to demonstrate the interface and prediction results.

## 🚀 How to Run the Project

The project was developed in Google Colab.

1. Clone or download this repository.
2. Open the `.ipynb` notebook in [Google Colab](https://colab.research.google.com/).
3. Download the dataset from Kaggle and upload or mount it in Colab.
4. Install any dependencies that are missing from the environment.
5. Run the notebook cells in order.
6. Train the model or load the saved model checkpoint.
7. Launch the Gradio interface to classify waste images.

**Note:** The dataset and trained model are not included in this repository. You must provide them separately before running the relevant notebook cells.

## 🔮 Future Enhancements

- Extend the dataset with more diverse real-world waste images.
- Improve classification performance for visually similar materials.
- Add multilingual disposal guidance.
- Explore real-time waste classification using a camera.
- Extend the system with object detection for images containing multiple waste items.

## ⚠️ Limitations

- The model predicts one primary category for an uploaded image; it does not detect and classify every individual object in a mixed image.
- Prediction confidence is not a guarantee of correctness.
- Disposal recommendations are general guidance and may vary by local recycling rules.
- Performance depends on image quality, lighting, background, and similarity to the training dataset.

## 👩‍💻 Project Information

**Project Name:** EcoSort – Smart Waste Classification Using MobileNetV2  
**Domain:** Deep Learning and Computer Vision  
**Purpose:** Academic mini-project

## 📄 License

A license has not yet been specified. If you intend to share or reuse this project publicly, consider adding an appropriate open-source license.

---

*EcoSort — Making waste classification smarter for a cleaner future. ♻️*
