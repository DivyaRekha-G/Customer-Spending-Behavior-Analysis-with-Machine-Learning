# Customer-Spending-Behavior-Analysis-with-Machine-Learning
This project builds a Linear Regression model to analyze and predict Yearly Amount Spent by E-Commerce customers. We explore how factors like Session Length, Time on App, Time on Website, and Membership Duration influence spending behavior.


📂 Dataset

Source: Kaggle (Ecommerce Customers Dataset)

File Used: Ecommerce_Customers.csv

Features:

Avg. Session Length

Time on App

Time on Website

Length of Membership

Target Variable: Yearly Amount Spent

🛠️ Libraries Used

pandas – For data manipulation

matplotlib & seaborn – For data visualization

scikit-learn – For machine learning models and evaluation

scipy.stats – For statistical analysis

math – For computing errors

🔍 Exploratory Data Analysis (EDA)

Display dataset summary (df.info(), df.describe()).

Visualized relationships using:

sns.jointplot() for feature correlation analysis.

sns.pairplot() for feature interactions.

sns.lmplot() to explore the effect of membership length.

🤖 Model Training

Feature Selection:

Independent Variables (X): Avg. Session Length, Time on App, Time on Website, Length of Membership

Dependent Variable (y): Yearly Amount Spent

Train-Test Split: 70% training, 30% testing (train_test_split())

Model Used: Linear Regression (LinearRegression() from sklearn)

Model Training:

.fit(X_train, y_train)

Extracted coefficients (lm.coef_)

📊 Model Evaluation

Predictions:

lm.predict(X_test) to get predictions.

Visualized predictions vs actual values using sns.scatterplot().

Performance Metrics:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

🔎 Residual Analysis

Plotted residual distribution using sns.displot().

Conducted a QQ plot to check normality of residuals (scipy.stats.probplot()).

📌 How to Run the Project

Clone the repository:

git clone https://github.com/yourusername/ml-ecommerce-regression.git
cd ml-ecommerce-regression

Install dependencies:

pip install pandas matplotlib seaborn scikit-learn scipy

Run the Jupyter Notebook or Python script to train and evaluate the model.

📈 Results & Insights

Length of Membership had the highest impact on yearly spending.

Time on App influenced spending more than Time on Website.

The model performed well, but additional features could further improve accuracy.

🔗 Connect & Contribute

If you found this project helpful, feel free to ⭐ the repo and contribute by improving the model or adding new insights! 

