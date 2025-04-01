# Skin Cancer Detection using CNN

This project uses a **Convolutional Neural Network (CNN)** to classify images of skin cancer into different categories. The dataset used is the **HAM10000 dataset**, which contains dermatoscopic images.

---

## 📊 Dataset
- **Dataset Name**: HAM10000
- **Source**: Kaggle
- **Features**:
  - `x`: Image pixel values (28x28 RGB images)
  - `y`: Labels indicating the type of skin cancer
- **Classes**:
  - `akiec`: Actinic keratoses and intraepithelial carcinomae
  - `bcc`: Basal cell carcinoma
  - `bkl`: Benign keratosis-like lesions
  - `df`: Dermatofibroma
  - `mel`: Melanoma
  - `nv`: Melanocytic nevi
  - `vasc`: Vascular lesions

---

## ⚙️ Requirements
The following libraries are used:
- `tensorflow`
- `keras`
- `sklearn`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `Pillow`
- `OpenCV`
- `imbalanced-learn`

Install the required libraries using:
```bash
pip install tensorflow keras sklearn pandas numpy matplotlib seaborn Pillow opencv-python imbalanced-learn
```

---

## 🛠️ Model Architecture
- **Sequential CNN model**
- Layers:
  - Conv2D → MaxPooling → Conv2D → MaxPooling → Flatten → Dense
  - Activation functions: `ReLU`, `Softmax`

---

## 🚀 Usage

### 1️⃣ Clone the Repository
```bash
git clone <your-repo-link>
cd skin-cancer-detection
```

### 2️⃣ Load the Dataset
Place the `HAM10000_metadata.csv` and `hmnist_28_28_RGB.csv` files in the directory or use Kaggle API to download them.

### 3️⃣ Run the Notebook
Run the `skin-cancer.ipynb` notebook in Google Colab.

### 4️⃣ Grad-CAM Visualization
The notebook includes **Grad-CAM** visualization, which generates heatmaps highlighting the regions of interest in the skin images.

---

## 📈 Results
- The model achieves **high accuracy** on the test dataset.
- The Grad-CAM heatmaps show the regions the model focuses on when making predictions.

---

## 📚 References
- [HAM10000 Dataset](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)
