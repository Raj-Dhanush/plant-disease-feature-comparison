# 🌱 Plant Disease Classification – Traditional vs Deep Learning Features  

## 📌 Overview  
This project is a **comparative study of feature extraction techniques** for plant disease classification using the **PlantVillage dataset**.  

- **Traditional feature extraction**: HOG, Local Binary Patterns (LBP), and Edge Detection.  
- **Deep learning–based feature extraction**: ResNet50, MobileNetV2, and VGG16 (pretrained CNN backbones).  
- **Classifiers used**: Logistic Regression, K-Nearest Neighbors (KNN), Decision Trees, and Random Forests.  

The objective is to analyze trade-offs in **performance, robustness, and generalization** between handcrafted features and deep CNN embeddings.  

---

## 📊 Key Results  

- 🏆 **Best Model:** MobileNetV2 + Logistic Regression → **94.8% accuracy, Kappa = 0.946**  
- 🥈 **Runner-up:** VGG16 + Logistic Regression → **91.5% accuracy, Kappa = 0.911**  
- 📈 **Best traditional feature:** HOG + Logistic Regression → **64.7% accuracy, Kappa = 0.629**  
- ⚠️ **Weakest features:** Edge detection and LBP, showing poor generalization (< 42% accuracy)  

---

## 📂 Repository Structure  
plant-disease-feature-comparison/
│── traditional_models.py      # HOG, LBP, Edge + ML classifiers
│── deep_learning_models.py    # ResNet50, MobileNetV2, VGG16 + ML classifiers
│── README.md                  # Project overview & documentation
│── requirements.txt           # Dependencies
│── results/                   # (Optional: metrics tables & plots)
