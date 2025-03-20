# 🌸📊 Flower Dataset Visualization & World Happiness Report Data Analysis  

## 📝 Project Overview  
This project explores **two distinct datasets** using **Python and Jupyter Notebook** to analyze patterns, correlations, and insights through data visualization techniques.  

### **📌 Objectives**  
1. **Flower Dataset Visualization**:  
   - Analyze the **Iris dataset** to explore relationships between petal and sepal dimensions.
   - Use **scatter plots, regression lines, and correlation matrices** to visualize patterns.
   - Compute the **Euclidean distance between species** based on petal and sepal characteristics.
   
2. **World Happiness Report Analysis**:  
   - Clean and preprocess happiness data from **2015-2019** reports.
   - Identify **correlation** between happiness score and other indicators (GDP, social support, etc.).
   - Apply **PCA (Principal Component Analysis)** to reduce dimensionality.
   - Visualize the global happiness score on an **interactive world map**.

---

# 📂 Dataset Information  

## **🌸 Flower Dataset (Iris Dataset)**  
- **Source:** Seaborn’s built-in `iris` dataset  
- **Records:** 150 samples  
- **Features:** Sepal length, Sepal width, Petal length, Petal width, and Species  
- **Goal:** Identify **species differences** using statistical and visual techniques.  

## **🌍 World Happiness Report**  
- **Source:** Kaggle - World Happiness Reports (2015-2019)  
- **Records:** 782 samples (before cleaning) → 710 samples (after removing missing values & zero-value rows)  
- **Features:** Country, Happiness Score, GDP, Social Support, Life Expectancy, Freedom, Corruption, Generosity  
- **Goal:** Identify **factors influencing happiness** and **perform PCA to reduce dimensions**.  

---

# 🛠️ Technologies Used  
- **Language:** Python  
- **Tools:** Jupyter Notebook  
- **Libraries:**  
  - **Pandas & NumPy** – Data Manipulation  
  - **Seaborn & Matplotlib** – Data Visualization  
  - **Plotly** – Interactive Data Visualization  
  - **Scipy** – Statistical Analysis  
  - **Scikit-Learn** – Principal Component Analysis (PCA)  

---

# 📊 Exploratory Data Analysis (EDA)  

## **🌸 Flower Dataset Visualizations**  

✅ **Pairwise Relationship Visualization**  
- Used **Seaborn’s `pairplot`** to visualize relationships between **petal & sepal dimensions**.  

✅ **Scatter Plots & Distance Calculation**  
- Analyzed **petal_length vs petal_width** and **petal_length vs sepal_width**.  
- Calculated **Euclidean distance** between **Setosa** and **Versicolor** species.  
- Overlaid **regression lines** to show trends.

📌 **Key Finding:**  
- Petal width and petal length showed the **strongest correlation** between species.  

✅ **Correlation Heatmap**  
- Generated a **correlation matrix** to identify which features are most related.  

📌 **Key Finding:**  
- **Petal Length & Petal Width** had the highest correlation in the dataset.  

### 📸 **Sample Visualization:**  
![Flower Data Visualization](images/iris_scatterplot.png)  

---

## **🌍 World Happiness Report Analysis**  

✅ **Data Cleaning & Preprocessing**  
- Combined **5 years (2015-2019)** of Happiness Reports.  
- Removed **missing data & zero-value countries**.  
- Grouped data by country & computed **average happiness score**.  

✅ **Correlation Analysis**  
- Used a **heatmap** to find relationships between variables.  
- **GDP** had the **strongest correlation** (0.81) with **Happiness Score**.  

✅ **Principal Component Analysis (PCA)**  
- Applied **PCA** to reduce **7 features → 5 principal components** while retaining **95.73% variance**.  
- **Score** was the **most influential** feature in PCA.  

✅ **World Happiness Map**  
- Created an **interactive choropleth map** to visualize **average happiness scores by country**.  

### 📸 **Sample Visualization:**  
![Happiness Report Map](images/happiness_map.png)  

---

# 📌 Key Insights  

### **🌸 Flower Dataset**  
- **Petal width & petal length are highly correlated**, meaning they are the most distinguishing features between species.  
- **Setosa & Versicolor species** show **significant differences in petal dimensions**, making them easier to classify.  

### **🌍 World Happiness Report**  
- **GDP & Social Support** had the highest correlation with **happiness scores**.  
- **Countries with the highest variance in happiness scores** include economically unstable regions.  
- **After outlier removal**, PCA results were **more stable**, confirming that the first **5 principal components** were enough to explain **most variance**.  

---

## Dependencies
- Python 3.x
- Jupyter Notebook
- pandas
- matplotlib
- seaborn

## Acknowledgments
This project was completed as part of the coursework for Data Visualization at Tennessee State University. Special thanks to the instructors and peers for their support and guidance.
