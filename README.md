# Building-and-Deploying-Churn-Prediction-Model-Using-IBM-Watson-Studio
This project demonstrates how to build and deploy a machine learning model using Watson Auto AI. Watson Auto AI allows you to build and deploy machine learning models without writing a single line of code, making it a powerful tool for quickly developing production-grade models.

# Introduction:
In this project, I developed a churn prediction model using IBM Watson Studio. Churn prediction is a critical task for businesses, as it helps them identify customers who are likely to leave and take proactive measures to retain them. I used the Telco Customer Churn dataset from Kaggle to train and deploy the model.

# Step-by-Step Guide:

## **Step 1:** Sign up for Watson Studio
Sign up for IBM's [Watson Studio](https://www.ibm.com/products/watson-studio?utm_content=SRCWW&p1=Search&p4=43700079344871072&p5=e&gad_source=1&gclid=CjwKCAjwh4-wBhB3EiwAeJsppDlIjD8B17O6lHYD5QOv_kuENe-wWW7GpYcUNOvJEd30YBj_bPzTiBoCDVwQAvD_BwE&gclsrc=aw.ds)

## **Step 2:**  Create a Project and Setup Watson Auto AI

**Create a Project:** Begin by creating a new project in IBM Watson Studio.</br>
<p><img src ="Images/Step2.JPG"</p></br>

**Add Auto AI Experiment:** Add a new Auto AI experiment to your project.</br>
<p><img src ="Images/Step2a.JPG"</p></br>

**Associate Machine Learning Service:** Associate a Watson Machine Learning service with your project. If you don't have one, you can create a new service.</br>
<p><img src ="Images/Step2b.JPG"</p></br>

## **Step 3:** Upload Your Data and Choose the Target
**Upload Dataset:** Upload your dataset to Watson Studio. For this project, I am using the [Telco Customer Churn Dataset from Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data?select=WA_Fn-UseC_-Telco-Customer-Churn.csv)</br>
<p><img src ="Images/Step3a.JPG"</p></br>

**Choose Target Variable:** Select the target variable for your model. In the Telco Customer Churn dataset, the target variable is 'Churn', which indicates whether the customer stays or leaves.</br>
<p><img src ="Images/Step3b.JPG"</p></br>

## **Step 4:** Run the Auto AI Experiment
**Run Experiment:** Start the Auto AI experiment. Auto AI will automatically select the most appropriate machine learning approach based on your dataset.</br>

<p><img src ="Images/Step4a.JPG"</p></br>
AutoAI doesn't just create a single model but explores and tunes multiple configurations for better performance. It explores various algorithms, tunes them for optimal performance, and creates different model configurations, ultimately presenting you with the best options for tackling customer churn.</br>

<p><img src ="Images/Step4c.JPG"</p></br>

**Evaluate Model Performance:** As the experiment runs, you can view the performance of the model in real-time. Auto AI will continue to tune the model to improve performance.</br>
<p><img src ="Images/Step4d.JPG"</p></br>

Finally, AutoAI evaluates all the generated pipelines (different combinations of algorithms, hyperparameter tuning, and feature engineering) based on metrics relevant to churn prediction, like AUC-ROC or F1 score. It then ranks them based on their performance, allowing you to choose the best option for deployment.</br>

<p><img src ="Images/Step4e.JPG"</p></br>

## **Step 5:** Deploy Your Auto AI Model
**Save the Model:** After the experiment, save the best-performing model for deployment. You can also save the experiment as a notebook for reproducibility or customization.</br>

<p><img src ="Images/Step5a.JPG"</p></br>

**Deploy the Model:** Watson Studio allows you to deploy the saved model as a web service. This enables real-time predictions on new data. Refer to the Watson Studio documentation for detailed deployment instructions covering various programming languages.
<p><img src ="Images/Step5b.JPG"</p></br>
<p><img src ="Images/Step5c.JPG"</p></br>
<p><img src ="Images/Step6b.JPG"</p></br>


## **Step 6:** Test the Model
Now it's time to test its mettle. You can feed the testing data into the model, and it generates churn predictions for the customer.  These predictions essentially indicate the likelihood of each customer churning in the future.</br>
Go to the deployments and select the model.
<p><img src ="Images/Step6a.JPG"</p></br>
Enter the input data and click on the "Predict" button.
<p><img src ="Images/Step6c.JPG"</p></br>
The results can be shown either in a tabular form or as a json view. The results can also be downloaded as a json file.
<p><img src ="Images/Step6d.JPG"</p></br>


By following these steps, you can quickly and efficiently build and deploy a machine learning model using Watson Auto AI. This project demonstrates the power of Auto AI in automating the machine learning model building process and making it accessible to users without extensive data science expertise.Remember, this is just a starting point – explore Watson Studio's documentation and tutorials to delve deeper into its functionalities and refine your churn prediction strategy.






