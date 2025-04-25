# German Bank Credit Risk Prediction

# 1. Description
- This is an end-to-end machine learning project using Random Forest to predict credit risk of German Bank's customers. It involves supervised learning (using a labeled training set) for classification, where the target is 1 if the customer represents a bad risk and 0 if he represents a good risk.
- I implemented this project following some CI/CD principles and using modular coding. First, I developed my entire analysis (from EDA to modeling) in notebooks. Then, I divided the project development into components responsible for data ingestion, transformation, and model training, following the same steps as in the notebooks. Once I had done this, I created scripts for automating the training and prediction pipelines using these components. The training pipeline executes them and obtains all the machine learning model artifacts, while the prediction pipeline makes predictions by consuming the obtained artifacts. All of this was made with good practices like virtual environment use (isolating dependencies), exception handling, loggings, documentation (every script/function/class purposes and definitions are defined inside the files), etc. Afterward, I built a web app in Flask, integrating everything mentioned above. My objective with this was to get closer to a real data science project workflow by packaging my entire project as a package.

# 2. Technologies and tools
- The technologies and tools used were Python (Pandas, Numpy, Matplotlib, Seaborn, Scikit-Learn, Category-Encoders, Scikit-Optimize, Xgboost, Flask), Jupyter Notebook, Git and Github (version control), machine learning classification algorithms, statistics, Anaconda (terminal) and Visual Studio Code (project development environment).

# 3. Business problem and project objective
Predict credit risk of German Bank's customers.

Credit risk refers to the potential financial loss that a lender, such as a bank, might incur if a borrower fails to repay a loan or credit obligation. It's the uncertainty about whether borrowers will honor their financial commitments.

The German Bank aims to predict their customers' credit risk for several reasons:

1. Risk assessment.
2. Profitability.
3. Minimize losses.
4. Compliance.
5. Customer segmentation.
6. Strengthen trust.

By employing predictive models, the bank can make informed decisions that balance profit generation with prudent risk management, ultimately benefiting both the institution and its customers. Thus, the project objective is to build a model that is able to identify as many as possible bad risk customers and provide valuable insights about credit risk within the available features. By doing this, the business problem is solved.

# 4. Solution pipeline
The following pipeline was used, based on CRISP-DM framework:

1. Define the business problem.
2. Collect the data and get a general overview of it.
3. Split the data into train and test sets.
4. Explore the data (exploratory data analysis)
5. Data cleaning and preprocessing.
6. Model training, comparison, selection and tuning.
7. Final production model testing and evaluation.
8. Conclude and interpret the model results.
9. Deploy.


# 5. Run this project on your local machine
Prerequisites:

Before getting started, make sure you have the following installed on your machine:
- Python 3.11.4
- pip (Python package manager)
- Git (Version control tool)

Once you have this installed, open a terminal on your local machine and run the following commands:

1. Clone the repository:
<pre>
https://github.com/SatyamSingh343/Credit_Risk_Management
</pre>

2. Navigate to the cloned repository directory:
<pre>
cd Credit_Risk_Management
</pre>

3. Create a virtual environment:
<pre>
python -m venv venv
</pre>

4. Activate the Virtual Environment:

Activate the virtual environment used to isolate the project dependencies.
<pre>
source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'
</pre>

5. Install Dependencies:

Use pip to install the required dependencies listed in the requirements.txt file.
<pre>
pip install -r requirements.txt
</pre>

6. Run the Application:
<pre>
python application.py
</pre>

7. Access the Project Locally:

After running successfully, you can access the project locally. Open a web browser and navigate to http://127.0.0.1:5000/

Then, go to the prediction page, select the input features values and click on submit. The prediction will appear on the right side.

7. Shutdown the Application:

To stop the application, you can typically press Ctrl+C in the terminal where the application is running.

8. Deactivate the Virtual Environment:

When you're done with the project, deactivate the virtual environment.

<pre>
deactivate
</pre>

# 6. Dataset link
The dataset was collected from kaggle and it belongs to UCI machine learning repository.

Link: https://www.kaggle.com/datasets/uciml/german-credit


