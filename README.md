**Retail Sales Forecast**
*Introduction*

In this project, we're diving into the world of retail sales prediction, where we use historical data to forecast future sales trends. It's like peering into a crystal ball to anticipate what customers will buy next, helping businesses make informed decisions and stay ahead in the competitive retail landscape.

*Table of Contents*

Key Technologies and Skills
Installation
Usage
Features
Contributing
License
Contact

*Key Technologies and Skills*

Python
Numpy
Pandas
Scikit-Learn
Plotly
Matplotlib
Seaborn
Pickle

*Installation*

To run this project, you need to install the following packages:

pip install numpy
pip install pandas
pip install scikit-learn
pip install xgboost
pip install plotly
pip install matplotlib
pip install seaborn

Features

Data Collection: Gather historical sales data, including dates, store information, holiday indicators, and markdown details for various products.

Data Preprocessing: Clean and preprocess the sales data, handle missing values, encode categorical variables, and format the data for analysis.

Data Understanding: The dataset comprises store, sales, and features data, offering details on store attributes like name, department, date, type, size, weekly sales, and environmental factors such as holiday status, temperature, fuel price, multiple markdowns, CPI, and unemployment. The primary focus is on predicting weekly sales, serving as the target variable for our modeling endeavors. This initial exploration forms the basis for subsequent data preprocessing and model development.

Exploratory Data Analysis (EDA): Perform EDA to understand sales patterns, identify trends, and explore the impact of holidays and markdowns on sales. Key analyses include:
Distribution of sales across stores and time periods.
Correlation between sales and holiday weeks, as well as markdown amounts.
Seasonal trends and fluctuations in sales performance.

Handling Null Values: Notably, the 'MarkDown' columns present a challenge with over 50% null values, while other columns exhibit minimal null values. To address this, we employ machine learning models to predict and impute the missing values, ensuring a more complete and robust dataset for subsequent analysis and modeling. This strategic approach allows us to mitigate the impact of missing data on the overall quality of our dataset.

Feature Improvement: Emphasizing enhanced modeling effectiveness, we concentrate on refining the dataset. This involves creating new features to extract deeper insights and enhance overall dataset efficiency. Evaluation, conducted through Seaborn's Heatmap, reveals that, a side from Size and Type with correlation values of 0.21 and 0.17 (absolute value) respectively, no other columns exhibit a strong correlation with weekly sales. This underscores the need for strategic feature enhancement to bolster the predictive power of our model.

*Machine Learning Regression Model:*

Multiple Models: Recognizing the challenge posed by over 50% null values in the 'MarkDown' columns, we adopt a comprehensive approach. Two separate machine learning models are trained to predict weekly sales – one leveraging the 'MarkDown' features and another excluding them. This dual-model methodology enables a thorough examination of the influence of 'MarkDown' columns on predictive accuracy, shedding light on the optimal approach for incorporating this information into the modeling process.

Algorithm Assessment: In the realm of regression, our primary objective is to predict the continuous variable of weekly sales. Our journey begins by splitting the dataset into training and testing subsets. We systematically apply various algorithms, evaluating them based on training and testing accuracy using the R2 (R-squared) metric, which signifies the coefficient of determination. This process allows us to identify the most suitable base algorithm tailored to our specific data.

Algorithm Selection: After thorough evaluation, two contenders, the Extra Trees Regressor and Random Forest Regressor, demonstrate commendable testing accuracy. Upon checking for any overfitting issues in both training and testing, both models exhibit strong performance without overfitting concerns. I choose the Random Forest Regressor for its ability to strike a balance between interpretability and accuracy, ensuring robust performance on unseen data.

Model Accuracy and Metrics: Upon optimizing parameters, model1 and model2 exhibit impressive accuracies of 97.4% and 97.7%, respectively. Opting for model1 (with MarkDowns) ensures robust predictions for unseen data. Additional evaluation includes key metrics like mean absolute error, mean squared error, root mean squared error, and the coefficient of determination (R-squared), offering a comprehensive assessment of the model's performance and reliability.


📧 Email: atchualagiri@gmail.com

