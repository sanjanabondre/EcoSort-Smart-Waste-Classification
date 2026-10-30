# 🌱 EcoSort – Smart Waste Classification using MobileNetV2

EcoSort is a deep learning-based waste classification system that automatically identifies different types of waste using image classification. It uses **MobileNetV2**, a lightweight Convolutional Neural Network (CNN) architecture, to classify waste images into six categories and provide appropriate disposal guidance.

The project aims to encourage proper waste segregation and promote environmentally responsible waste management.

## ✨ Features

- 📸 **Image Classification:** Upload a waste image for automatic classification.
- 🧠 **MobileNetV2 Model:** Uses transfer learning for efficient image recognition.
- ♻️ **Six Waste Categories:** Classifies waste into:
  - Cardboard
  - Glass
  - Metal
  - Paper
  - Plastic
  - Trash
- 📊 **Prediction Confidence:** Displays the model's confidence score.
- 🌍 **Disposal Recommendations:** Provides category-specific waste disposal guidance.
- 🖥️ **Interactive Interface:** Built using Gradio for easy interaction.

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- MobileNetV2
- NumPy
- Matplotlib
- Scikit-learn
- Gradio
- Google Colab

## 📂 Dataset

The project uses the **Garbage Classification Dataset**, containing six categories of waste images.

| Category | Number of Images |
|---|---:|
| Cardboard | 403 |
| Glass | 501 |
| Metal | 410 |
| Paper | 594 |
| Plastic | 482 |
| Trash | 137 |
| **Total** | **2,527** |

The dataset was divided into training, validation, and testing sets.

- Training: 1,766 images
- Validation: 377 images
- Testing: 384 images

## 🧠 Model Development

The project uses MobileNetV2 with transfer learning to classify waste images.

The model development process includes:

1. Loading and exploring the dataset.
2. Image preprocessing and resizing.
3. Splitting the dataset into training, validation, and testing sets.
4. Applying data augmentation.
5. Training and fine-tuning the MobileNetV2 model.
6. Evaluating classification performance.
7. Saving the trained model for predictions.

## 📈 Model Performance

| Metric | Result |
|---|---:|
| Initial Test Accuracy | 82.00% |
| Final Test Accuracy | **83.07%** |

The final model achieved an improvement of 1.07 percentage points over the initial model.

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/sanjanabondre/EcoSort-Smart-Waste-Classification.git
```

### 2. Navigate to the Project Folder

```bash
cd EcoSort-Smart-Waste-Classification
```

### 3. Install Dependencies

```bash
pip install tensorflow numpy matplotlib scikit-learn gradio pillow
```

### 4. Run the Application

If the application file is named `app.py`:

```bash
python app.py
```

Alternatively, open the Google Colab notebook and execute the cells in sequence.

## 📁 Project Structure

```text
EcoSort-Smart-Waste-Classification/
│
├── EcoSort.ipynb
├── app.py
├── waste_classifier_final.keras
├── README.md
└── requirements.txt
```

*Note: Adjust the file names and structure according to the files actually included in the repository.*

## 🔮 Future Scope

- Improve classification accuracy with additional training data.
- Extend the system to identify multiple waste objects in a single image.
- Integrate the system with smart waste collection and segregation solutions.
- Expand waste categories for more comprehensive classification.

## 👩‍💻 Author

**Sanjana Bondre**

- GitHub: [@sanjanabondre](https://github.com/sanjanabondre)
- LinkedIn: [Sanjana Bondre](https://linkedin.com/in/sanjana-bondre-086327287)

## 🌿 Conclusion

EcoSort demonstrates how deep learning and computer vision can contribute to smarter waste classification. By combining MobileNetV2 with an interactive interface, the project makes waste identification and disposal guidance more accessible.
