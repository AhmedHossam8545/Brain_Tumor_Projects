# 🧠 Brain Tumor Classification & Segmentation  

This project was developed as part of my course with **Instant Software Solutions**.  
It implements two deep learning pipelines to help in the **detection and localization of brain tumors from MRI images**:  

- **Classification**: EfficientNetB3 model classifies MRI scans as either **Tumor** or **No Tumor**.  
- **Segmentation**: U-Net model segments and highlights the tumor region in the MRI image.  

---

## 🚀 Features
- Upload an MRI image and get a **tumor/no tumor prediction** with confidence score.  
- Generate a **segmentation mask** for the tumor region.  
- Interactive **Streamlit web application** for end-to-end usage.  

---

## 🛠️ Tech Stack
- **Python 3.10+**  
- **TensorFlow / Keras**  
- **EfficientNetB3** (classification)  
- **U-Net** (segmentation)  
- **OpenCV** (image preprocessing)  
- **Streamlit** (deployment)  

---

## 📂 Project Structure
```
├── app.py                        # Streamlit deployment script  
├── brain_tumor_best_model.h5     # Trained EfficientNetB3 model for classification  
├── final_unet.keras              # Trained U-Net model for segmentation  
├── data/                         # MRI dataset (yes/no folders for classification)  
├── notebooks/                    # Training notebooks for classification & segmentation  
├── requirements.txt              # Dependencies  
└── README.md                     # Project documentation  
```

---

## ⚙️ Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/brain-tumor-classifier-segmentation.git
cd brain-tumor-classifier-segmentation
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Run the Streamlit app**
```bash
streamlit run app.py
```

---

## 📊 Dataset
- Classification dataset consists of **two folders**:  
  - `yes/` → MRI scans with tumor  
  - `no/` → MRI scans without tumor  
- Segmentation dataset consists of MRI scans with corresponding **ground truth masks**.  

> ⚠️ Dataset not included in repo due to size. You can download from [Kaggle Brain Tumor MRI Dataset](https://www.kaggle.com/datasets) or use your own.  

---

## 🔎 Results
- **Classification Accuracy**: Up to **94–100%** on test set.  
- **Segmentation**: U-Net produces binary masks highlighting tumor regions.  

---

## 📌 Future Improvements
- Train on **larger datasets** for robustness.  
- Explore **EfficientNetV2 / Transformers** for better accuracy.  

---

## 🙏 Acknowledgements
- Developed during my course with **[Instant Software Solutions](https://www.linkedin.com/company/instant-software-solutions/)**  
- Thanks to open-source contributors and Kaggle for datasets.  

---

## 📜 License
This project is for **educational purposes only** and should not be used for real-world clinical decisions without further validation.  
