# Movie Recommendation System
## 1.0 Project Overview
This project involves analysis of movies data to build a recommendation system model that provides diverse options and accurate recommendations to customers that improves their shopping experience and increase engagement with shop catalogs, subsequently increasing sales. The research follows cross industry standard procedures (CRISP-DM) methodlogy fo the movies industry.

## 2.0 Business Understanding
In the midst of modern business competion,the new film shop purposes to increase its customer interaction by providing personalized recommendations of individual films. This recommendation system will be important for improvement in customer experience, increase customer engagement and driving sale. By offering personal suggestions based on customers' preferences, previous behavior and film ratings, the shop expects to increase customer engagement, increase sales and improve customer retention.

## 2.1 Business Objective
A new movie shop opens a branch in a new town with an aim to invent better interaction with customers by offering personalized movie recommendations. The company aims to recommend movies in which the customers have shown interest, liked, or even inquired about. This customized service will expose the customer to films they might not have considered but will likely enjoy based on the films they browse or inquire about. It would, therefore, be able to provide personalized recommendations through customer data on movie preference, past queries, and behavior to enhance customer experience, thereby commanding high satisfaction, loyalty, and repeat visits.

**General Objective**

* To build a model that provides top 5 movie recommendations to a user, based on their ratings of other movies.
  
## 3.0 Data Sources and Understanding
### The Data
The dataset for modelling was drawn from https://grouplens.org/datasets/movielens/latest/.
Merged dataset contains 100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users.

### Content

* **userId:** Unique identifier for the user.

* **movieId:** Unique identifier  for movie.

* **rating:** Ratings given by the user to the movie.

* **timestamp:** Time at which the rating was given by user.

* **title:** Name of the movie.

* **genres:** The genres for which movies belong.

* **tag:** A glimpse of what the movie is about or like.
  
## 4.0 Data Preparation.
This is the process of cleaning data in readiness for analysis and it involves the following:

* **Validity check;** Checking for irrelevant features and removing them or selecting the revelant features
* **Data completeness;** Checking for missing values and treating them.
* **Data accuracy;** Checking for outlier values in the data that distorts its accuracy.
* **Data consistency;** Consistency is achieved through removal of duplicates in the dataframe.
* **Data Uniformity;** Involves feature engineering

## 5.0 Modelling

### Modelling Approach
* Item-based Collaborative Filtering recommendation model,
* Content-based Filtering recommendation model,
* Matrix Factorization with Singular Value Decomposition(SVD) model.

## 5.1 Data Visualizations.

1. Distribution of Movie ratings
   
   ![image](https://github.com/user-attachments/assets/1ffadaa3-b354-4d01-bc4f-62fe4dc3ccf4)

2. Count Plot for movie distribution by genre.

   ![image](https://github.com/user-attachments/assets/bce9d321-3804-4325-b0ff-ac9a0475ee2f)


## 5.2 Findings

The best performing model for deployment is Matrix Factorization with Singular Value Decomposition (SVD).
The metrics of comparison were mean squared error(MSE) and mean absolute error (MAE).

### 5.2.1 Model performance
1. Visualization of error residuals for model performance.

   ![image](https://github.com/user-attachments/assets/21a26f82-6b10-42a3-83d7-9a3cbf8228bb)

2. Receiver Operating Characteristic (ROC) Curve, Area under the Curve (AUC) visual. This shows performance of the model in terms of accuracy.

   ![image](https://github.com/user-attachments/assets/138a099c-e301-49a0-a944-20f65d011a7c)


## 5.3 Use Case
* Clone this repository:

* bash

* Copy code

* git clone https://github.com/Felix-87/Phase4_project.git

* Run index.ipynb in Jupyter Notebook or any other compatible IDE.


## 6.0 Conclusions and Recommendations

Best recommendtion system model for deployment is **Matrix Factorization with Singular Value Decomposistion(SVD)** by the movie shop. 

Model performance with an AUC (Area Under the Curve) = 0.99 indicates that the model highly distinguishes between relevant and irrelevant recommendations, which translates to higher precision and higher recall. The model ranks the relevant movies higher in the list, ensuring that the user gets personalized and accurate recommendations.

This ensures that;
* It best recommends movies based on what customers have done, liked, or searched (personalized recommendations).
* Help customers discover movies that they may have never considered but might like and thus increase their tastes and knowledge of films.
* Incentivize customers to spend more time on the website with value-added recommendations relevant to their interests.
* Personalized suggestions will increase sales and improve customer retention, as they will revisit your site for more and remain longer-term.
* Facilitate an easy and smooth recommendation experience for your customers.




