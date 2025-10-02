🖼️ Celebrity Face Recognition using Machine Learning

This project is my first hands-on exploration of image-based machine learning. I built a small celebrity face recognition system to classify between Gigi Hadid, Bella Hadid and Kendall Jenner, focusing on image preprocessing, feature engineering, and classical ML models.

Unlike many template projects, this was built out of personal interest and curiosity — it gave me my first real exposure to working with images and strengthened my foundation in computer vision and machine learning pipelines.

🔹 Project Overview

Objective: Build a simple face recognition system using machine learning.

Dataset: Custom-collected images of Gigi Hadid, Bella Hadid & Kendall Jenner.

Approach:

Face detection with Haar cascades

Feature extraction using raw pixels + wavelet decomposition (DWT)

Dimensionality reduction with PCA

Classification using SVM, Random Forest, Logistic Regression, and KNN

Best Model: SVM with Linear Kernel (approx. 75% accuracy).

🔹 Methodology

Dataset Preparation

Images collected and organized by class (Gigi,Bella,and Kendall).

Face Detection & Cropping

Detected faces using Haar cascade classifiers.

Cropped valid face regions for consistency.

Feature Extraction

Raw pixel features (32×32 grayscale).

Wavelet features capturing high-frequency edges and textures.

Concatenated both into a single feature vector.

Feature Scaling & PCA

Normalized features.

Applied PCA to reduce dimensionality while retaining variance.

Model Training & Evaluation

Trained SVM, Random Forest, Logistic Regression, and KNN.

Used GridSearchCV with cross-validation for tuning.

Evaluated with accuracy, F1-score, and confusion matrices.

Prediction on New Images

Created preprocessing function for unseen test images.

Final model predicts celebrity label (Gigi, Bella or Kendall).

🔹 Results & Key Learnings

Learned that images can be decomposed into different frequency bands (high/low frequency).

Understood multilevel decomposition and how wavelets capture texture details.

Got hands-on with try-except blocks for robust coding.

Improved my understanding of data structures, algorithms, and ML pipelines.

Discovered that image ML isn’t just about training models, but also about cleaning data, extracting features, and building systematic workflows.

🔹 Tech Stack

Languages: Python

Libraries: OpenCV, NumPy, PyWavelets, Scikit-learn, Matplotlib

Concepts: Haar Cascade, DWT, PCA, SVM, Random Forest, Logistic Regression, KNN

🔹 Future Directions

This project was a stepping stone for me into computer vision. In the future, I aim to:

Experiment with deep learning models (CNNs) for better accuracy.

Extend to multi-class celebrity classification.

Explore applications in medical imaging and high-dimensional data, which connect with my research interests .
