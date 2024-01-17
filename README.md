#### Introduction

The project focuses on analyzing customer reviews from a Women’s Clothing E-Commerce dataset. It aims to derive insights from review texts, classify them as recommendations or not, and understand customer preferences and sentiments. The dataset comprises 23,486 reviews, each with several features like age, review text, rating, and recommendation status. 

#### Here is the tableau dashboard link to understand the data
(https://public.tableau.com/app/profile/tirth.gala7456/viz/ClothingE-commerceReview/ReviewAnalysis)

#### Understanding spreadsheet data

This 23486 rows and 10 feature variables. Each row corresponds to a customer review, and includes the variables:

1. Clothing ID: Integer Categorical variable that refers to the specific piece being reviewed.

2. Age: Positive Integer variable of the reviewers age.

3. Title: String variable for the title of the review.

4. Review Text: String variable for the review body.

5. Rating: Positive Ordinal Integer variable for the product score granted by the customer from 1 Worst, to 5 Best.

6. Recommended IND: Binary variable stating where the customer recommends the product where 1 is recommended, 0 is not recommended.

7. Positive Feedback Count: Positive Integer documenting the number of other customers who found this review positive.

8. Division Name: Categorical name of the product high level division.

9. Department Name: Categorical name of the product department name.

10. Class Name: Categorical name of the product class name.

#### Data Preparation
The initial phase involved cleaning and preprocessing the dataset. Unnecessary columns like 'Age', 'Unnamed: 0', 'Clothing ID', 'Rating', 'Positive Feedback Count', 'Title', and 'Unnamed: 0' were dropped to focus on the textual review and recommendation indication. Missing values in 'Class Name', 'Division Name', and 'Department Name' were handled by dropping such entries.
#### Feature Engineering
A new feature, 'Review_length', was created to analyze the length of each review. The recommendation indicator was converted from binary to a string format for better interpretability ('Positive' for 1 and 'Negative' for 0). The text was further processed by removing non-alphanumeric characters, converting to lowercase, and removing stopwords.
#### Exploratory Data Analysis
Descriptive statistics were used to understand the review lengths. The longest and shortest reviews were identified for insights. A word cloud was generated to visualize the most frequent words in the reviews, providing a graphical representation of the data's textual elements.
#### Model Building and Evaluation
Two models, Logistic Regression and Random Forest, were trained on the processed text. The text data was vectorized using CountVectorizer, transforming it into a format suitable for model input. The models were evaluated based on accuracy, with Logistic Regression achieving an accuracy of approximately 88% and Random Forest around 86%.
#### LSTM Neural Network
An LSTM (Long Short-Term Memory) model was also developed to handle the sequence nature of text data. The model consisted of an embedding layer, LSTM layer, and a dense layer with sigmoid activation. It was trained on tokenized and padded sequences of the reviews. The model achieved an accuracy of around 89% on the test set.
#### Predictions on Unseen Data
The models were tested on new textual data to predict their recommendations. Different outcomes from the models highlighted the varied interpretations and responses to the unseen data.
#### Challenges and Learnings
1. Data Cleaning: The initial challenge was cleaning and preprocessing the dataset, requiring decisions on which features to keep or drop.
2. Text Processing: Implementing text processing techniques like tokenization and stopwords removal was critical to prepare the data for modeling.
3. Model Selection and Tuning: Choosing and tuning the right models to handle textual data was a significant learning curve.
4. Interpreting Results: Understanding and interpreting the model outputs, especially the differences in predictions between models, provided insights into their strengths and weaknesses.

#### Future Scope
Future enhancements can include integrating more sophisticated NLP techniques, experimenting with other deep learning architectures, and exploring sentiment analysis for a more nuanced understanding of customer reviews.
