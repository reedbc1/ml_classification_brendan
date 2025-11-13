# Peer Review  
[Link to reviewed file](https://github.com/ssowers2/ml_classification_sowers/blob/main/notebooks/project01/classification_sowers.ipynb.ipynb)

## Clarity & Organization  
The introduction clearly described the data and the project objective. Headings were numbered and bold, making it easy to follow the flow of the notebook. Reflections summarized the takeaways of each section.

## Feature Selection & Justification  
Sowers decided to use all features in model training, noting that "mushroom edibility depends on a number of physical traits". I agree that the more information used that can separate muchrooms from one another, the better the classification model is likely to perform.  

Sowers said that some features are expected to be highly predictive of edibility, such as odor, spore_print_color, and ring_type, because they directly relate to characteristics used to identify poisonous mushrooms. Though more difficult to show with categorical variables, it would be informative to try to measure correlation or frequencies between these features and the target variable to show which variables have the most prediction value. To visualize this, a chart showing the decision tree nodes and leaves might be helpful, but the number of columns (because of OneHotEncoder) and the number of features could made it difficult to read.  

Sowers listed the increase in feature count due to OneHotEncoding (24 to 94 columns) to be one of the challenges she faced. She could consider using numerical encoding to still have only 24 features. This would make it easier to interpret visualizations of the model's decision making process and decrease training time. However, the one hot encoded data will be useful if she later decides to try logistic regression. Regression models could numerically encoded labels as having meaning (ex. 2 is greater than 1), which may not correctly reflect the data, so OneHotEncoder would be the best choice.

## Model Performance & Comparisons  
Sowers clearly explained their findings. She concluded that the data is highly seperable because both a decision tree and random forest model were able to achieve 100% accuracy. Because random forest handles variability well, Sowers indicated it would be her preferred choice of model. She also suggests applying feature importance analysis as a next step, which would verify the features she expected to be most predictive. She also suggests the importance of testing the models on additional data to ensure that overfitting isn't responsible for their 100% accuracy.

## Reflection Quality  
Insights were well thought out. Sowers provided solid reasoning for her decisions, summarized findings, and clearly explained her interpretation of the results. She suggested next steps to further validate and improve her work.
