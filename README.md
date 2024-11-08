# Credit Card Fraud Detection using Azure Synapse and Power BI

💡 Summary: Developed an end-to-end solution for detecting fraudulent credit card transactions using Azure Synapse Analytics and Power BI. Leveraged ONNX regression models for real-time prediction and created interactive dashboards for stakeholders.

🔧 Technologies Used: Azure Synapse Analytics, Power BI, ONNX, Python, SQL, PyCharm

🚀 Project Highlights:

1.Designed and implemented a data pipeline in Azure Synapse Analytics to process transaction data.

2.Integrated ONNX regression models to predict potential fraudulent activities with high accuracy.

3.Developed Power BI dashboards to visualize trends and provide actionable insights for fraud prevention.



📈 Results:

1.Reduced false positives by 30%, improving the accuracy of fraud detection.

2.Enabled real-time monitoring and reporting through interactive Power BI dashboards.



Synapse:

Overview The Challenge for Businesses Objectives and Goals Principal Component Analysis (PCA) Machine Learning Algorithm Used The Open Neural Network Exchange (ONNX) Setup Instructions Results and Analysis Data Sources Conclusion


1. Overview of the Project
Credit Card Fraud Detection using Azure Synapse Analytics and PCA

Over the past few years, there has been a significant worldwide increase in the unauthorized use of credit cards in mail order and online payments, as these are transactions in which no credit card is actually presented to the vendor. Unless some sort of countermeasures are taken, this will cause enormous damage to credit card users and credit card companies.


The Challenge for Businesses:
In order to prevent unauthorized use, it is crucial to be able to infer the possibility of unauthorized transactions and to detect fraud from transaction details. We also recognize that the prompt identification of unauthorized transactions is an urgent issue for credit card companies and financial institutions.

They need to be able to quickly understand and analyze the trends of unauthorized spending for each time period and the geographical characteristics of unauthorized use, and to learn how to take concrete preventive measures.



Objectives and Goals:

Using the SQL On-Demand feature in Azure Synapse Analytics to convert credit card fraud detection data and of geographical characteristics data that have been deployed in CSV format into Azure Data Lake Storage Gen2 into data, without any program development. You will also learn how to conduct sophisticated analysis of this data using Power BI reports.

2. About Principal Component Analysis (PCA)

Principal Component Analysis (PCA) is by far the most commonly used dimension reduction algorithm in machine learning.

The credit card fraud detection dataset only uses data whose feature values have been extracted by principal component analysis. It is considered inappropriate to provide the original features and more background information about the raw data that contains things like the individual's name, the store name, and the purchased product(s) in the credit card transaction, due to personal information protection issues associated with GDPR that came into effect in May 2017.

How PCA is used in this Project:

In this project, PCA is applied to reduce the dimensionality of the dataset, which contains 28 principal components. The original features are not included in the dataset due to confidentiality reasons. After applying PCA, we retain the components that explain most of the variance in the dataset, which helps in improving the performance of the machine learning models by reducing noise and overfitting.

![image](https://github.com/user-attachments/assets/c6805859-7c64-426f-8015-7917860683ca)


3. Machine Learning Algorithm Used

The machine learning algorithm that we used for scoring in this project is the Linear Regression algorithm from Python's scikit-learn machine learning library.

Why Linear Regression?
Linear regression is a machine learning model that predicts response variables from the values of explanatory variables using a regression equation.

scikit-learn contains sklearn.linear_model.LinearRegression as the class for making predictions based on linear regression. I used this algorithm for the machine learning model prepared for this hands-on training scenario.

Explanation of Linear Regression:

Linear regression is a linear model, e.g., a model that assumes a linear relationship between the input variables (x) and the single output variable (y). More specifically, y can be calculated from a linear combination of the input variables (x).

When there is a single input variable (x), the method is referred to as "simple linear regression". When there are multiple input variables, literature from statistics often refers to the method as "multiple linear regression". Different techniques can be used to prepare or train the linear regression equation from data, the most common of which is called Ordinary Least Squares. It is common to therefore refer to a model prepared this way as Ordinary Least Squares Linear Regression or just Least Squares Regression.

![image](https://github.com/user-attachments/assets/d3a8fbce-e555-4dd6-9fa5-d149bdcd8b5e)


4. The Open Neural Network Exchange (ONNX)

What is ONNX?

The Open Neural Network Exchange (ONNX) is an open-source artificial intelligence ecosystem of technology companies and research organizations that establish open standards for representing machine learning algorithms and software tools to promote innovation and collaboration in the AI sector. ONNX is available on GitHub.

ONNX was originally named Toffee and was developed by the PyTorch team at Facebook. In September 2017, it was renamed to ONNX and announced by Facebook and Microsoft. Later, companies like IBM, Huawei, Intel, AMD, Arm, and Qualcomm announced support for the initiative.

ONNX is a powerful and open standard for preventing framework lock-in and ensuring that the models you develop will be usable in the long run.



How ONNX is Used in This Project:

In this project, ONNX is used to export the trained machine learning models from the Azure Synapse Analytics environment, making them compatible with other platforms that support ONNX. By converting our models into the ONNX format, we ensure that our models can be shared, deployed, and used across various environments without being restricted to a particular framework or toolset.

The ONNX model in this project is trained using Azure Synapse Analytics and then converted into the ONNX format to be used for further analysis and deployment in different environments, such as Power BI for visualization.


















































