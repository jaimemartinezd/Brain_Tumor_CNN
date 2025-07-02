# 🧠 Brain Tumor Detection CNN

This repository contains a Deep Learning project for **brain tumor detection** from medical images, using a **CNN based on EfficientNetB0**.

The goal is to classify images into four categories:
- `glioma_tumor`
- `meningioma_tumor`
- `pituitary_tumor`
- `no_tumor`

---

## 📁 Project structure

```
├── data/
│   ├── Training/
│   │   ├── glioma_tumor/
│   │   ├── meningioma_tumor/
│   │   ├── pituitary_tumor/
│   │   └── no_tumor/
│   └── Testing/
│       ├── glioma_tumor/
│       ├── meningioma_tumor/
│       ├── pituitary_tumor/
│       └── no_tumor/
├── models/
│   └── best_model_ENB0.keras
├── notebook/
│   └── brain_tumor_detection.ipynb
├── requirements.txt
├── LICENSE
└── README.md
```

- data/: Contains the training and testing images, organized by classes.

- models/: Stores trained models.

- notebook/: Contains the complete workflow.

- requirements.txt: All the required dependencies to run the project.

- LICENSE: License of the project.

---

### 📦 Requirements

To install the dependencies, run:

pip install -r requirements.txt

---

### 🧰 Technologies

Python

TensorFlow: to build and train the CNN.

EfficientNetB0: optimized pretrained architecture.

OpenCV: for image processing.

Matplotlib & Seaborn: for data visualization.

NumPy: for data handling and analysis.

---

### ⚙️ How the model works

Data loading: Images are read from the Training and Testing folders. Added generators for data augmentation.

Preprocessing: Images are resized and normalized to match EfficientNetB0 input requirements.

Model building: EfficientNetB0 is used as the base model. Custom dense layers and regularization layers are added for classification.

Training: The model is trained using the images in the Training set, doing a train_test_split.

Evaluation: Model performance is evaluated using the Testing set.

---

### 📊 Expected results

Accuracy and loss plots during training.

Confusion matrix and classification metrics (accuracy, recall, F1-score).

All steps, results and plots are documented in the notebook.

---

###  🗂️  Data Source

The data used in this project comes from the [Brain Tumor Classification MRI dataset on Kaggle](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri).

---

### ✏️ Author

This project was developed by Jaime Martinez as a practice exercise in Deep Learning.

---

### ✅ License

This project is licensed under the MIT License.
You are free to use, modify and share it — please cite this repository if you find it useful.

---

### ⭐ Contributing
Pull requests are welcome!
If you’d like to improve the model, add visualizations, or enhance the documentation, feel free to contribute.

---

## 📬 Contact
If you have any questions or suggestions, open an issue in this repository or get in touch directly.
