# Document-Classification
This module automatically identifies and classifies financial documents such as Aadhaar cards, PAN cards, and cheques. It uses a Convolutional Neural Network (CNN) to process and recognize images, enabling efficient and accurate document verification.
# 📊 Recommendation System – FinAI Advisor

## 🚀 Overview
This module is a Hybrid Recommendation System developed as part of the FinAI Advisor project. It suggests relevant financial products to users based on their profile and preferences.

The system combines:
- Content-Based Filtering
- Collaborative Filtering (SVD / Matrix Factorization)

to generate personalized recommendations.

---

## 🎯 Objective
To recommend suitable financial products such as loans, credit cards, and insurance by analyzing:
- User financial attributes (income, credit score, age)
- Historical user-product interactions (ratings)

---

## 🧠 Methodology

### 1. Content-Based Filtering
- Matches user attributes with product requirements
- Filters products based on:
  - Minimum income
  - Minimum credit score

### 2. Collaborative Filtering
- Uses user-item interaction matrix
- Applies SVD (Singular Value Decomposition)
- Predicts ratings based on similar users

### 3. Hybrid Approach
- Combines both methods:
  - Content-based → eligibility filtering
  - Collaborative → ranking relevance

---

## 📂 Dataset

### Users
- user_id
- income
- credit_score
- age

### Products
- product_id
- product_name
- min_income
- min_credit_score

### Ratings
- user_id
- product_id
- rating

---

## ⚙️ Implementation Steps
1. Data preprocessing  
2. Create user-item matrix  
3. Apply SVD model  
4. Generate predicted ratings  
5. Apply content-based filtering  
6. Combine results and rank  
7. Return top recommendations  

---

## 📈 Model Evaluation
- Metric used: RMSE (Root Mean Squared Error)
- Achieved RMSE ≈ 1.5

Since recommendation systems predict ratings, RMSE is used instead of accuracy.

---

## 💡 Output
Top recommended financial products with labels:
- ⭐ Highly Recommended
- 👍 Good Option
- ⚠️ Consider

---

## 🖥️ Deployment
- Integrated using Streamlit
- Takes user input:
  - Existing user → User ID
  - New user → Income, Credit Score, Age
- Displays recommendations instantly

---

## 🧪 Sample Output

Recommended Products:
- ⭐ Personal Loan – Highly Recommended  
- 👍 Credit Card – Good Option  
- ⚠️ Car Loan – Consider  

---

## 🚀 Future Improvements
- Use real-world datasets  
- Improve cold-start problem  
- Add deep learning models  
- Enhance UI/UX  

---

## 👩‍💻 Author
Pratibha Mishra  
Machine Learning Intern  
Project: FinAI Advisor  

---

## ⭐ Conclusion
This module demonstrates how hybrid recommendation systems can provide personalized financial suggestions and can be extended into a full-scale financial advisory system.
