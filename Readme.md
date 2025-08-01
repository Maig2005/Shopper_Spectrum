Shopper Spectrum: Customer Segmentation and Product Recommendation

An interactive **Streamlit dashboard** that helps visualize customer behavior, perform **RFM-based customer segmentation**, and recommend similar products using **collaborative filtering**. Ideal for E-commerce or Retail analytics teams to explore customer value and personalize offerings.

---

## Features

 **Exploratory Data Analysis (EDA)**
- 15 detailed charts covering univariate, bivariate, and multivariate analyses.
- Understand trends in purchases, prices, customer countries, and basket behavior.

 **Customer Segmentation**
- Predict a customer’s segment using RFM (Recency, Frequency, Monetary) scores.
- Uses **KMeans clustering** trained on your historical transaction data.

 **Product Recommendation**
- Enter a product name to get **top 5 similar items** based on customer co-purchase behavior.
- Built using **item-item collaborative filtering**.

---

## Project Structure

shopper_spectrum/
├── app/ # For internal application utilities
├── data/ # CSV datasets (cleaned_retail_data.csv)
├── models/ # Saved KMeans model, scaler, similarity matrix
│ ├── kmeans_model.joblib
│ ├── rfm_scaler.joblib
│ └── product_similarity.pkl
├── visuals/ # 15 EDA charts (PNG format)
├── streamlit_app/
│ └── app.py # Main Streamlit dashboard
└── README.md