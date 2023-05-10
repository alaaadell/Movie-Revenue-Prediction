# Movie-revenue-prediction
## Preprocessing Techniques:
#### We grouped the voice actors into a list by the movie name.
#### Then we fill the directors and the voice actors with an API with a TMDb library because the nulls of the directors was 428 and the nulls of the voice actors was 424.
#### The release date column: We take only the year and convert the data type into int.
#### The director column: We apply frequency encoder and apply  KNN imputer to find the rest of NULLS (19 values), now the director column has no nulls.
#### The voice actor column: We apply frequency encoder and apply  KNN imputer to find the rest of NULLS (19 values), now the voice actor has no nulls.
#### The MPAA-Rating column: We make one hot encoder for PG, PG-13, and other-rating. The nulls will be in other-rating column with value 0.
#### The genre column: We make one hot encoder for Comedy,  Adventure, Drama and other-genre. The nulls will be in other-genre column with value 0.
## Feature Selection:
we dropped the movie-name column because each name is unique, character column because all of them are almost unique, and applied pval algorithm to choose the most suitable features that fits with the label.
## Classification models:
#### Logistic Regression
#### Adaboost classifier with decision tree classifier 
#### Random Forest classifier 

![image](https://user-images.githubusercontent.com/71910329/179068886-877cbd77-28c4-433c-92d1-314ff5042321.png)

![image](https://user-images.githubusercontent.com/71910329/179069008-66da6f4b-e79a-428d-85e5-139aee82da50.png)

![image](https://user-images.githubusercontent.com/71910329/179069064-d85c9aa9-f1fc-4f91-8e6a-291436707c42.png)

## Regression models
#### Multivariable linear regression
#### Polynomial regression
#### Linear regression using Cross validation





