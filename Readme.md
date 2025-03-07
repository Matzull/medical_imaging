# 🚀 Image Classification Project with PyTorch

Welcome to the **Image Classification Project**! This repository is designed for training deep learning models using **PyTorch**, with a strong focus on **image preprocessing** and **classification** (both **binary** and **multi-class**).

---

## 📁 Project Structure

```
.
├── data/                   # Dataset directory (raw & preprocessed)
│   ├── train/              # Training dataset
│   │   ├── 0/              # Class 0 images
│   │   ├── 1/              # Class 1 images
│   │   ├── 2/              # Class 2 images
│   │   ├── 3/              # Class 3 images
│   │   ├── 4/              # Class 4 images
│   ├── test/               # Test dataset
│   │   ├── 0/              # Class 0 images
│   │   ├── 1/              # Class 1 images
│   │   ├── 2/              # Class 2 images
│   │   ├── 3/              # Class 3 images
│   │   ├── 4/              # Class 4 images
│   ├── prep/               # Preprocessed images
├── notebooks/
│   ├── preprocess.ipynb    # Notebook for image preprocessing
│   ├── main.ipynb          # Main notebook for model training
├── models/                 # Saved trained models
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
```

---

## ⚙️ Installation & Dependencies

To get started, install the required dependencies using:

```sh
pip install -r requirements.txt
```

🚨 **Note:** A **CUDA-enabled GPU** is required for efficient model training.

---

## 🖼️ Data Preprocessing

The preprocessing pipeline, implemented in `preprocess.ipynb`, includes:

✅ **Image Resizing** – Standardizing image dimensions.
✅ **Background Removal** – Cleaning up unnecessary background noise.
✅ **Data Augmentation** – Enhancing the dataset with transformations like:
   - Horizontal & Vertical Flips
   - Brightness & Contrast Adjustments
   - Gaussian Blur for smoother features

To generate preprocessed data, run the `preprocess.ipynb` notebook.

---

## 🏋️ Model Training

The training workflow, managed in `main.ipynb`, consists of:

1️⃣ **Loading preprocessed images** into PyTorch DataLoaders.
2️⃣ **Defining the model architecture** for classification.
3️⃣ **Configuring hyperparameters** such as batch size & epochs.
4️⃣ **Training the model** using GPU acceleration.
5️⃣ **Evaluating performance** on the test dataset.

### 🔧 Configuration

Key parameters defined in `main.ipynb`:

- `IMG_DIR` → Path to preprocessed images.
- `BATCH_SIZE` → Number of images per batch.
- `EPOCHS` → Total training iterations.
- `BINARY` → Enable/disable binary classification.

---

## 📊 Results & Metrics

The training notebook (`main.ipynb`) outputs:

📌 **Confusion Matrix** – Visualizing misclassifications.
📌 **ROC-AUC Curves** – Measuring model confidence.
📌 **Classification Reports** – Evaluating precision, recall, and F1-score.

---

## 🤝 Contribution & Contact

💡 Want to contribute? Feel free to **open an issue** or **submit a pull request**!

For any inquiries or suggestions, reach out! 🚀

---

This project is crafted to make **image classification experimentation** easy and efficient with **PyTorch**. Happy coding! 😃

