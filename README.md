# 👗 Women Boutique Image Recommendation System  
**(CNN • Transfer Learning • Embeddings • Flask Deployment)**

## 📌 Project Overview
This project is an **end-to-end image-based recommendation system** for women’s fashion products.  
Given an input dress image, the system recommends **visually similar products** using **CNN feature embeddings** and **cosine similarity**.

The solution covers the **complete ML lifecycle**:
- Data preprocessing
- Model training & fine-tuning
- Embedding generation
- Similarity-based recommendation
- Web deployment using Flask

---

## 🎯 Problem Statement
Traditional product recommendations rely on text or user history.  
This project solves the **cold-start problem** by recommending fashion items **purely based on image similarity**.

---

## 🧠 Approach & Methodology
1. **Dataset Preparation**
   - Used `styles.csv` metadata and women apparel images
   - Filtered relevant women clothing categories

2. **Model Architecture**
   - Base Model: **MobileNetV2 (ImageNet weights)**
   - Custom Head:
     - Convolution Layer
     - Global Average Pooling
     - Dense embedding layer
   - Transfer learning + fine-tuning of top layers

3. **Embedding Generation**
   - Extracted fixed-length embeddings for each image
   - Stored embeddings for fast similarity search

4. **Recommendation Logic**
   - Generated embedding for uploaded query image
   - Used **cosine similarity** to find Top-K similar images

5. **Deployment**
   - Flask web application
   - Image upload → recommendation display
   - Public access via **ngrok** (Google Colab)

---

## 🧰 Tech Stack
- **Python**
- **TensorFlow / Keras**
- **MobileNetV2**
- **NumPy, Pandas**
- **Scikit-learn (cosine similarity)**
- **Flask**
- **HTML + CSS**
- **Google Colab + ngrok**

---


