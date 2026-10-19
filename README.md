Customer Segmentation Using Clustering
Project Description
Customer Segmentation Using Clustering is a machine learning web application that groups customers according to similar characteristics and behavior. It helps businesses understand customer types and plan suitable marketing strategies.

The application uses clustering algorithms to find groups in customer data and displays charts, model comparisons, customer personas, business insights, and predictions for new customers.
Features
- Customer data dashboard and data exploration
- Data preprocessing, missing-value handling, duplicate removal, and outlier handling
- Feature scaling using StandardScaler or MinMaxScaler
- Elbow method and Silhouette Score to help choose the number of clusters
- K-Means, Hierarchical Clustering, and Gaussian Mixture Model (GMM)
- Model evaluation using Silhouette Score, Davies-Bouldin Score, and Calinski-Harabasz Score
- PCA-based visualization of customer groups
- Customer personas and marketing recommendations
- Prediction of the segment for a new customer
- User registration and login with a SQLite database
Technologies Used
- Python
- Streamlit
- Pandas and NumPy
- Scikit-learn
- Plotly
- SQLite
- bcrypt
Project Files
- main.py — runs the Streamlit application
- customers.csv — sample customer dataset
- data_preprocessing.py — loads and prepares data
- clustering.py — clustering algorithms, evaluation, and predictions
- database.py — user registration, login, and database operations
- ui_components.py — reusable interface components
- customer_segmentation.db — SQLite database file created/used by the application
Requirements
Install Python 3.10 or later, then install the required packages:
pip install streamlit pandas numpy scikit-learn plotly bcrypt
How to Run
1. Download or clone this repository.
2. Open a terminal in the project folder (the folder containing main.py).
3. Install the packages listed above.
4. Start the application:
streamlit run main.py
5. Open the local URL shown in the terminal, usually http://localhost:8501.
Dataset
The application uses customers.csv by default. You can explore the available columns in the app and select suitable numeric features for clustering. The results depend on the dataset and the features selected.
How It Works
1. Load customer data.
2. Explore the data and check its quality.
3. Clean missing values, duplicates, and outliers as needed.
4. Scale the selected features.
5. Choose a suitable number of clusters.
6. Train and compare clustering models.
7. View the customer segments and business insights.
8. Enter details for a new customer to predict a segment.
Important Notes
- Clustering is an unsupervised learning technique, so the dataset does not need predefined customer labels.
- Do not upload real customer personal information, passwords, or other sensitive data to a public repository.
- For a public GitHub repository, consider excluding the SQLite database file if it contains real user information. Add local database files and Python cache folders to .gitignore.
Future Enhancements
- Deploy the app to a cloud hosting service.
- Add more clustering algorithms and model evaluation options.
- Improve customer segment reports and export features.
