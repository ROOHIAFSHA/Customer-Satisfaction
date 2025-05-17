# 📊 Customer Satisfaction Prediction
## 📁 Project Overview
This project aims to predict Customer Satisfaction Ratings (on a scale from 1 to 5) based on customer support ticket data. The data includes customer demographics, product information, ticket details, response/resolution times, and more.

Using machine learning, we build a model that helps companies understand the key drivers of satisfaction and proactively improve their support experience.

## 📌 Dataset Description
The dataset includes customer support tickets for various tech products. Key features include:

Feature Name	Description
Customer Age	Age of the customer
Customer Gender	Gender of the customer
Product Purchased	Tech product purchased
Ticket Type	Type of support request (e.g., technical issue, billing inquiry)
Ticket Status	Status of the ticket (e.g., open, closed)
Ticket Priority	Priority assigned to the ticket (low, medium, high, critical)
Ticket Channel	Channel through which the ticket was raised (email, phone, chat, etc.)
First Response Time	Time taken to respond initially (in minutes or hours)
Time to Resolution	Total time taken to resolve the issue (in hours/days)
Customer Satisfaction Rating	Target variable (1–5 rating)

## 🧠 Problem Statement
Build a classification model that predicts the Customer Satisfaction Rating using other ticket-related features.

## 🛠️ Tools & Technologies
Python

Pandas, NumPy for data manipulation

Matplotlib, Seaborn for data visualization

Scikit-learn for machine learning

## 🧾 Steps Performed
Data Import & Inspection

Load CSV file

View structure and summary using .info() and .describe()

Missing Value Handling

Dropped rows where target variable (Customer Satisfaction Rating) was missing

Dropped rows with any remaining missing feature values

Feature Selection & Encoding

Selected meaningful features

Encoded categorical variables using LabelEncoder

Train/Test Split

Split data into training and testing sets (80/20 ratio)

Model Training

Used RandomForestClassifier for multi-class classification

Trained model on training data

Model Evaluation

Confusion Matrix

Classification Report (Accuracy, Precision, Recall, F1-Score)

Feature Importance Visualization

Plotted which features most influence satisfaction prediction

## 📈 Results
The model outputs classification performance metrics.

A bar chart visualizes feature importance — helping us understand what drives customer satisfaction most (e.g., resolution time, priority, etc.).

## 📌 Use Cases
Proactively improve support: Focus on features causing low satisfaction.

Ticket triaging: Assign resources better based on predicted satisfaction risk.

Customer retention: Identify unhappy customers early.

## ✅ Future Improvements
Combine NLP techniques on Ticket Description to extract sentiment/intent.

Group ratings into categories (e.g., Low, Medium, High) for simplified classification.

Use more advanced models (e.g., XGBoost, GridSearchCV for tuning).

Build a dashboard for live prediction & monitoring.

## 📁 How to Run
bash
Copy
Edit
# 1. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# 2. Run the Python script
python customer_satisfaction_prediction.py
