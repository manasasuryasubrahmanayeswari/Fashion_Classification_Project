#  Fashion Classification Project using CNN

##  Project Overview  
This project is a **deep learning-based fashion classification system**.  
Using a **Convolutional Neural Network (CNN)**, it classifies fashion product images (shirts, jeans, watches, etc.) into their **categories** such as *Apparel, Footwear, Accessories*, etc.  

The dataset used is the **Fashion Product Images (Small) Dataset** (from Kaggle – Myntra).  
The project demonstrates **end-to-end machine learning workflow**: data preprocessing, CNN model training, evaluation, and visualization.  

---

##  Objectives
- Build a **multi-class CNN classifier** for fashion product categories.  
- Achieve high accuracy in predicting **masterCategory** from images.  
- Visualize **training vs validation accuracy & loss curves**.  
- Prepare the model for **future extensions** like subcategory classification or trend analysis.  

---

##  Dataset
- **Source**: [Fashion Product Images Dataset - Small (Kaggle)](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)  
- **Size**: ~44,000 product images + metadata (CSV).  
- **Columns include**:  
  - `id` → Image ID (maps to image filename)  
  - `gender` → Men, Women, Boys, Girls, etc.  
  - `masterCategory` → Apparel, Footwear, Accessories, etc.  
  - `subCategory`, `articleType`, `baseColour`, `season`, `year`, etc.  


---

##  Tech Stack
- **Programming Language**: Python  
- **Libraries**: TensorFlow/Keras, Pandas, NumPy, Matplotlib, scikit-learn  
- **Environment**: Google Colab / Jupyter Notebook  
- **Version Control**: Git + GitHub  

---

##  Implementation Steps
1. **Data Preprocessing**
   - Loaded metadata (`styles.csv`).  
   - Filtered missing/invalid data.  
   - Linked images with metadata using `id`.  
   - Encoded labels (`masterCategory`).  
   - Applied data augmentation using `ImageDataGenerator`.  

2. **Model Development**
   - Built a CNN with layers:  
     - Convolution + MaxPooling  
     - Dropout & Batch Normalization  
     - Fully Connected Dense layers  
   - Used **Adam optimizer** and **SparseCategoricalCrossentropy loss**.  

3. **Training**
   - Training set: ~35,000 images  
   - Validation set: ~8,800 images  
   - Epochs: 10  
   - Batch size: 32  

4. **Evaluation**
   - Achieved **~98% Validation Accuracy**  
   - Plotted accuracy & loss curves.  
   - Generated classification report & confusion matrix.  

---

##  Results

- **Final Training Accuracy**: ~97%  
- **Final Validation Accuracy**: ~98%  


##  How to Run

### 🔹 Clone the Repository
```bash
git clone https://github.com/your-username/Fashion_Classification_Project.git
cd Fashion_Classification_Project
``` 
### 🔹 install dependencies
``` bash
pip install -r requirements.txt

