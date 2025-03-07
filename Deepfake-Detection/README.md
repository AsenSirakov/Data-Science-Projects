# Computer Vision: Detecting Deepfake Images  

## 📺 Project Overview  
With the rise of **generative AI**, distinguishing real images from AI-generated ones is crucial for **digital forensics, misinformation detection, and media authenticity verification**. This project explores **deep learning-based deepfake image detection** using **ResNet-50, ConvNeXt-Tiny, and EfficientNet-B0**, leveraging **transfer learning** and **Grad-CAM visualization** to enhance interpretability.  

## 🚀 Key Contributions  
- **Model Benchmarking & Optimization:** Compared **ResNet-50, ConvNeXt-Tiny, and EfficientNet-B0** for deepfake detection.  
- **Preprocessing & Augmentation:** Cleaned, normalized, and augmented data to enhance model reliability.  
- **Computational Efficiency:** Implemented **GradScaler & autocast** for **mixed-precision training acceleration**.  
- **Model Explainability:** Used **Grad-CAM & Multi-layer Grad-CAM** to interpret AI decisions.  
- **Performance Evaluation:** Measured **accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrices**.  
- **Generalization Challenges:** Addressed **dataset diversity and confidence calibration** to improve robustness.  
- **Experiment Tracking:** Monitored training with **TensorBoard** for better insights.  

---

## 🛠️ Technologies & Libraries Used  
- **Python**  
- **PyTorch, Torchvision** → Deep learning & CNNs  
- **Pandas, NumPy** → Data manipulation  
- **Matplotlib, Seaborn** → Data visualization  
- **Grad-CAM, TensorBoard** → Model explainability & experiment tracking  
- **Scikit-learn** → Performance evaluation metrics  

---

## 📂 Dataset Information  
The data is acquired through **Kaggle** and is **free for use**. The dataset consists of **authentic images sampled from the Shutterstock platform** across various categories, including a **balanced selection where one-third of the images feature humans**. These authentic images are **paired with AI-generated equivalents** created using **state-of-the-art generative models**.

This structured pairing enables a **direct comparison between real and AI-generated content**, providing a robust foundation for developing and evaluating **image authenticity detection systems**. The dataset is the official dataset for the **2025 Women in AI Kaggle Competition**.

### **Dataset Details:**  
- **Creators:** Alessandra Sala, Margarita Pitsiani, Manuela Jeyaraj, Toma Ijatomi  
- **License:** Apache 2.0  
- **Link to Data:** [Kaggle Dataset](https://www.kaggle.com/datasets/alessandrasala79/ai-vs-human-generated-dataset/data)  

---

## 📂 Dataset(Test_set_v1) and ConvNext model:
The original test set was replaced by the new test_set_v2, so here is a link to the data and the model.
**Google Drive:** [Project data and model](https://drive.google.com/drive/folders/1YgW9GoGYvqR1Uexz53lEmYPNNzXpw_4c?usp=sharing)

---

## 📊 Key Insights & Findings  

### **1️⃣ Deepfake Detection Performance**  
- **ConvNeXt-Tiny** achieved the **best classification accuracy**, outperforming **ResNet-50 & EfficientNet-B0**.  
- **Misclassification of AI-generated content in the latest test set(test_set_v2)**, requiring **adaptive decision thresholds**.  
- **Grad-CAM visualizations** highlight critical regions used for classification.   

### **2️⃣ Dataset & Generalization Challenges**  
- **Lack of dataset diversity** impacts model robustness against **new AI-generated techniques**.  
- **Confidence calibration needed** for better uncertainty estimation.  

### **3️⃣ Future Work (Currently working on it)**  
#### **Dataset Expansion:**  
- Incorporate **more diverse AI-generated images** from various sources (**GANs, Diffusion models, etc.**).  
- Apply **hard negative mining** to expose the model to **challenging deepfake examples**.  

#### **Confidence Calibration & Threshold Tuning:**  
- Implement **Platt scaling or isotonic regression** to improve uncertainty estimation.  
- Experiment with **adaptive classification thresholds** instead of a static 0.5 cutoff.  

#### **Architectural Improvements:**  
- Test **Vision Transformers (ViTs) or larger ConvNeXt models** for enhanced feature extraction.  
- Explore **self-supervised learning** to improve representations for real vs. AI-generated images.  

#### **Improved Explainability:**  
- Use **SHAP, LIME, or attention-based heatmaps** to better understand **why certain deepfakes are misclassified**.  

---

## ▶️ How to Run the Project  

### **1. Clone the Repository**  
```bash
git clone https://github.com/AsenSirakov/Data-Science-Projects.git
cd Deepfake-Detection
```

### **2. Open the Jupyter Notebook**  
Run the following command to start Jupyter Notebook:  
```bash
jupyter notebook Ai_vs_real_images_classification.ipynb
```
### **3. Download the original test_data from the Google drive and the convnext model if you don't want to train it yourself**
- Open the google drive via the link and donwload the data and the model. [Project data and model](https://drive.google.com/drive/folders/1YgW9GoGYvqR1Uexz53lEmYPNNzXpw_4c?usp=sharing)

### **4. Execute the Notebook**  
- Run all cells sequentially.  
- The notebook covers **data preprocessing, model training, evaluation, and Grad-CAM visualization**.  

---

