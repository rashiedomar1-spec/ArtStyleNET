# 🖼️ ArtStyleNet: Artistic Style Similarity with Deep Learning

ArtStyleNet explores how deep learning can uncover hidden patterns in artworks and quantify artistic style similarity.  
The project demonstrates how computational methods can approximate the intuitive “feeling” of style similarity that humans perceive, enabling art recommendation systems and broader appreciation of art.

---

## 📌 Project Overview

**Goal**: Detect stylistic similarity across paintings by analyzing visual features.  

**Approach**: Feature extraction → dimensionality reduction → clustering → visualization.  

**Why**: Traditional style recognition is subjective and expert-driven; this project makes it more accessible for general audiences.

---

## ⚙️ Methodology

**Feature Extraction (ResNet)**  
Used pre-trained ResNet to capture features such as brushstrokes, textures, and color composition.  

**Dimensionality Reduction (PCA)**  
Reduced high-dimensional feature vectors into interpretable components while minimizing noise.  

**Clustering (LDA)**  
Grouped artworks into latent style clusters.  
Explored 5–10 clusters, evaluated via perplexity & elbow method.  

**Visualization (Heatmaps)**  
Generated heatmaps showing style distributions across artworks.  
Identified stylistic variability among painters.

---

## 📊 Dataset

**Source**: 🎨 [Dacon Artist Classification Competition](https://dacon.io/en/competitions/official/236006/data)  
**Size**: 5,910 paintings by 51 artists  
- Includes metadata (artist, year, genre, nationality), but only images were used  
- Training set only (evaluation dataset excluded)  

⚠️ *Dataset is not included in this repository due to size limitations. Please download directly from the official Dacon link.*

---

## 📂 Repository Structure

ArtStyleNET/
│── ARTWorkClassification.ipynb # Main notebook for classification
│── Feature_Extraction.ipynb # Feature extraction with ResNet
│── main.py # Python script entry point
│── artists_info.csv # Metadata: artists’ info
│── train.csv # Training dataset (download from Dacon)
│── test.csv # Test dataset (download from Dacon)
│── open/ # Folder for extracted/generated outputs
│── ArtStyleNet (Final exam project).pptx # Presentation slides
│── ArtStyleNet - Content-based recommendation.pdf # Report

---

## 📈 Results

- Identified hidden style clusters beyond traditional categories.  
- Heatmap visualizations revealed variability in stylistic influences.  
- Produced top artworks per cluster and artist distributions.  

---

## 🧩 Limitations & Future Work

- PCA assumes linearity → future work could test AutoEncoders or t-SNE for non-linear relationships.  
- Only visual features considered → integrating metadata (genre, nationality) could enhance results.  
- Could be extended into personalized art recommendation systems.  

---

## 📑 References

- Gatys et al., 2016 – CNNs for style transfer  
- Karayev et al., 2014 – Predicting artistic styles  
- Saleh & Elgammal, 2015 – Visual style similarity  
- Van Der Maaten & Hinton, 2008 – t-SNE for visualization  
- Elgammal et al., 2018 – Creative Adversarial Networks  
- Tan et al., 2020 – Self-supervised clustering  

---

## 🙋 Author

Developed by **Omar Rashid** as part of exploring deep learning in artistic style recognition a
