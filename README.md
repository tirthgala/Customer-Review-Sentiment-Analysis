#### Introduction ####

The project focuses on analyzing customer reviews from a Women’s Clothing E-Commerce dataset. It aims to derive insights from review texts, classify them as recommendations or not, and understand customer preferences and sentiments. The dataset comprises 23,486 reviews, each with several features like age, review text, rating, and recommendation status. 

#### Here is the tableau dashboard link to understand the data
(https://public.tableau.com/app/profile/tirth.gala7456/viz/ClothingE-commerceReview/ReviewAnalysis)
#### Inside repository
1. Women Clothing Review Analysis (pdf): This file has the business report of the whole project. It includes information right from data preparation to final business application of the project.
2. Women_Clothing_Reviews_Code (ipynb): This file contains the code of the whole project i.e., right from data preparation to testing model performance
3. Women Clothing E-commerce Reviews (csv): File contains raw data downloaded from Kaggle
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

#### Conclusion
The project successfully utilized different machine learning models to analyze customer reviews from an e-commerce platform. The LSTM model, in particular, showed promising results in understanding and predicting customer recommendations. This project demonstrates the potential of machine learning in extracting valuable insights from textual data, which can be pivotal for businesses in understanding customer sentiments and preferences.
