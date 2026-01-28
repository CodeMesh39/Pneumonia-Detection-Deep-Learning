🫁 Pneumonia Detection from Chest X-Ray Images using Deep Learning

An end-to-end deep learning system for automated pneumonia detection from chest X-ray images using ResNet50 transfer learning and Grad-CAM explainability.

📌 Project Overview

Pneumonia is a serious respiratory infection that can be life-threatening if not detected early. This project builds an AI-based medical image classification system that can assist in identifying pneumonia from chest X-ray scans.

The system leverages transfer learning with a pre-trained ResNet50 model and incorporates Grad-CAM visual explanations to highlight lung regions influencing the model’s decision.

🧠 Key Features

🔍 Automated pneumonia detection from X-ray images

🏥 Medical image classification using deep learning

♻️ Transfer learning with ResNet50

🎯 Fine-tuning for improved performance

📊 Full model evaluation with medical metrics

🔥 Grad-CAM visual explanations for interpretability

🗂 Dataset

Source: Kaggle Chest X-Ray Pneumonia Dataset
Providers: NIH Clinical Center & Guangzhou Women and Children's Medical Center

The dataset contains chest X-ray images categorized into:

Normal

Pneumonia

Dataset is not included in this repository due to size and licensing.

🏗 Model Architecture

Base Model: ResNet50 (ImageNet pretrained)

Input Size: 224 × 224

Transfer Learning with frozen base layers

Fine-tuning of top convolutional layers

Output Layer: Binary classification (Normal vs Pneumonia)

⚙️ Technologies Used

Python

TensorFlow / Keras

NumPy, Matplotlib, Seaborn

OpenCV

Google Colab

📊 Model Evaluation

The model was evaluated on an unseen test set using:

Accuracy

Precision

Recall (Sensitivity)

Specificity

Confusion Matrix

ROC Curve (AUC)

Medical emphasis was placed on high recall for pneumonia cases to reduce false negatives.

🔬 Model Explainability (Grad-CAM)

Grad-CAM was used to visualize which lung regions influenced the model’s predictions.

🧪 Pneumonia Case

🧪 Normal Case

These heatmaps show the model focuses on clinically relevant lung areas, increasing trust and transparency.

📁 Repository Structure
notebooks/
│
├── 01_Model_Training_Pneumonia.ipynb
├── 01B_FineTuning_Continuation.ipynb
├── 02_Model_Evaluation.ipynb
└── 03_GradCAM_Explainability.ipynb

gradcam_results/
├── gradcam_pneumonia.png
└── gradcam_normal.png

▶️ How to Run

Download the dataset from Kaggle

Place dataset in Google Drive or local path

Run notebooks in order:

Model Training

Fine-Tuning

Evaluation

Grad-CAM Explainability

🎯 Applications

AI-assisted pneumonia screening

Medical image analysis research

Healthcare AI systems

Clinical decision-support tools

🚀 Future Improvements

Train on larger, more diverse datasets

Multi-class classification (viral vs bacterial pneumonia)

Deployment as a web app for clinical use

Ensemble models for improved robustness

👨‍💻 Author

Deep Learning & Medical AI Enthusiast
Project developed as part of an academic and portfolio deep learning initiative.

⭐ If you found this project interesting, consider giving it a star!
