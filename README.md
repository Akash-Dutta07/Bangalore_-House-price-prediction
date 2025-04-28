

![Image](https://github.com/user-attachments/assets/fb0acb8a-089e-46c1-8d79-ac5fc4c84bda)

This project builds a machine learning model to predict house prices in Bengaluru, one of India's fastest-growing cities. Using a publicly available dataset, the project focuses on data cleaning, feature engineering, and model training with various regression algorithms. The model predicts property prices based on features like location, total square footage (total_sqft), number of bedrooms, number of bathrooms, etc, and other amenities, helping buyers and investors make informed decisions.














## **📄Description**


In this project, price was used as the dependent variable for predictive modeling.
A total of 5 machine learning models — Linear Regression, Ridge Regression, Random Forest, Lasso Regression, and Gradient Descent — were trained.
Among them, Gradient Boosting Machine (GBM) achieved the best performance with an R² score of 0.73754.


 **Dataset Overview:**

This dataset contains 13,320 records of residential properties in Bengaluru, India.
It includes the following features:

- area_type: Type of area (e.g., Super built-up, Plot, etc.)

- availability: Property availability status (e.g., Ready To Move, Launch date)

- location: Location of the property

- size: Number of bedrooms (BHK)

- society: Name of the society (many missing values)

- total_sqft: Total area (in square feet)

- bath: Number of bathrooms

- balcony: Number of balconies

- price: Price of the property (in lakhs)

Note:

Some features like society, bath, and balcony have missing values.



## **📥Datasets**


The dataset is available here..

https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data

## **📋Conclusion**

Initially, the Gradient Boosting Regressor achieved a Train R² score of 0.87758 and a Test R² score of 0.73754, with an RMSE of 48.43.
Since the test accuracy was relatively low compared to the training accuracy, backward elimination was applied on a copy of the dataset (df2) to identify and remove less important features like area_type. After dropping it and re-running the model, the performance was reassessed.
Finally, GBM was re-tried on the refined dataset, aiming to improve the model’s ability to generalize and predict property prices more accurately.
## **🔧Requirements**

- Python
- Pandas & NumPy
- scikit-learn
- Matplotlib & Seaborn






## 🚀 How to Use This Repository

You can run this project directly on **Google Colab** without setting up anything locally:

### ✅ Steps:

1. **Clone the repository** to your system:
   ```bash
   git clone <repository-url>
   ```
   Replace `<repository-url>` with the actual link to this repo.

2. Go to [Google Colab](https://colab.research.google.com/)

3. Click on **File > Upload notebook**  
   and upload the `.ipynb` file from the cloned folder and run the file




