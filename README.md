# 🛒 Retail Basket Analysis using Python

This project performs **Market Basket Analysis** on a retail dataset to identify frequently bought-together products and generate **association rules**. It uses **Python (Pandas, NumPy, and itertools)** for data preprocessing and analysis.

---

## 📊 Project Overview

The goal of this project is to understand customer purchasing patterns by finding relationships between products purchased together.  
This helps businesses with:
- Product placement optimization  
- Cross-selling strategies  
- Marketing and promotion planning  

---

## 🧠 Key Concepts

- **Market Basket Analysis** – a data mining technique used to uncover relationships between products.
- **Association Rules** – derived using the **Apriori algorithm** to identify frequent itemsets.
- **Support, Confidence, Lift** – statistical metrics to measure rule strength and relevance.

---

## ⚙️ Technologies Used

- **Python 3**
- **Pandas** – Data preprocessing and manipulation  
- **NumPy** – Numerical computation  
- **Matplotlib / Seaborn** – Data visualization  
- **itertools** – Efficient combination generation  

---

## 📁 Dataset

The dataset contains customer transaction information, including:
- **Invoice / Order ID**
- **Product / Item Description**
- **Quantity Purchased**
- **Customer ID**
- **Country**

Each transaction represents products purchased together in one order.

---

## 🔍 Steps Performed

1. **Data Loading & Cleaning**
   - Removed missing and duplicate records  
   - Standardized column names and formats  

2. **Data Transformation**
   - Created a one-hot encoded “basket” of products  
   - Transformed quantity data into binary (1 = purchased, 0 = not purchased)

3. **Frequent Itemset Generation**
   - Computed support for 1-item and 2-item combinations  

4. **Association Rule Mining**
   - Derived rules like:
     > If a customer buys *X*, they are likely to buy *Y*.

5. **Visualization**
   - Bar chart and pie chart for top-selling items  
   - Network graph of product associations  

---

## 🧩 Example Insights

```
If a customer buys ['milk'], they are likely to buy ['bread'] (confidence: 0.72)
If a customer buys ['butter'], they are likely to buy ['jam'] (confidence: 0.65)
```

---

## 🚀 How to Run This Project

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Retail-Basket-Analysis.git
   cd Retail-Basket-Analysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Run the cells in sequence to reproduce results.

---

## 🧾 Output Files

- `Retail_Basket_Analysis.ipynb` – main notebook  
- `online_retail_customer_churn.csv` – dataset (optional)  
- `frequent_itemsets.csv` – list of frequent item combinations  

---

## 📈 Future Improvements

- Implement **Apriori** or **FP-Growth** algorithm from `mlxtend`  
- Add **interactive visualizations** using Plotly or NetworkX  
- Extend to **real-time retail data streams**  

---

## 👨‍💻 Author

**Reddy Deekshith**  
📧 your-email@example.com  
🌐 https://github.com/your-github-username

---

⭐ *If you find this project useful, consider giving it a star on GitHub!*
