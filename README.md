# 🛒 Synthetic Customer Profiles for AI-Driven Product Recommendations in E-Commerce  

✨ *AI-powered synthetic customer profiles and reviews for smarter e-commerce recommendations.*  


## 📌 Overview  
This project generates **synthetic customer profiles and product reviews** using **GPT-2** to support **AI-driven product recommendation systems** in e-commerce.  
It creates realistic datasets, visual insights, and automated customer feedback for:  
- 📊 Data analysis  
- 🤖 Model training  
- 🔒 Privacy-preserving testing (without real customer data)  


## 🚀 Features  
- Load and analyze an e-commerce dataset (CSV)  
- Generate plots:
  - Product **Category Distribution**  
  - **Region-wise Revenue**  
- Build customer review prompts (from dataset or custom)  
- Generate synthetic reviews using **HuggingFace GPT-2**  
- Save generated reviews and dataset summaries  

## 📂 Repository Structure  
ecom-gpt2-reviews/
│── generate_ecom_profiles_gpt2_only_improved.py # Main script
│── requirements.txt # Dependencies
│── README.md # Documentation
│── data/ # (optional) Sample input CSV
│── plots/ # Auto-generated plots
│── outputs/ # Generated reviews
│── prompts.txt # (optional) Custom prompts

 

## ⚙️ Installation  

Clone this repository:  
git clone https://github.com/<Ritikakeshtwal>/ecom-gpt2-reviews.git
cd ecom-gpt2-reviews


python -m venv venv
venv\Scripts\activate

Usage
Basic Run
python generate_ecom_profiles_gpt2_only_improved.py \
  input-csv data/synthetic_ecom_customers_gpt2.csv \
  plots-dir plots \
  reviews-csv outputs/generated_reviews_gpt2.csv

  Options

prompts-file prompts.txt → Load prompts from file

from-dataset → Auto-build prompts from dataset columns

num-reviews 50 → Control number of reviews

model-name gpt2 → Choose model (gpt2, distilgpt2, etc.)

cpu → Force CPU even if GPU is available

Example Outputs

plots/category_distribution.png – Product category distribution

plots/region_revenue.png – Region-wise revenue

outputs/generated_reviews_gpt2.csv – AI-generated reviews

plots/dataset_summary.txt – Summary of dataset
