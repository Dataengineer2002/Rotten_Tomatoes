# Rotten_Tomatoes
Predicting Audience Rating in Rotten Tomatoes Dataset using Neural Network and XGBRegressor

**Rotten Tomatoes Audience Rating Prediction Model**

This model predicts the audience rating of movies based on various features from the Rotten Tomatoes dataset, which includes movie details such as title, genre, director, cast, runtime, critics' consensus, and other key metadata. The target variable for prediction is the 'audience_rating' column, which represents the user-generated score for each movie.

To achieve this prediction, we implemented two distinct machine learning models:

1. **Neural Network Model**: A deep learning approach is used to capture complex, non-linear relationships within the data. The neural network is trained on multiple features of the dataset and aims to learn patterns that might not be immediately apparent through traditional models. The architecture consists of an input layer, several hidden layers with activation functions to capture non-linearity, and an output layer that generates the predicted audience rating.

2. **XGBRegressor Model**: This model utilizes a gradient boosting algorithm that is particularly effective for regression tasks. XGBoost is known for its high performance and scalability, allowing the model to make accurate predictions even with a large number of features. By focusing on boosting weak learners, XGBRegressor can identify important features and make more precise predictions, improving model accuracy.

**Model Pipeline and Workflow:**
- **Data Preprocessing**: Handling missing values, encoding categorical features (such as genre, studio name, and directors), and scaling numeric features (such as runtime and ratings).
- **Feature Engineering**: Additional features like text length in 'movie_info' and 'critics_consensus' are created to enrich the model input.
- **Model Selection and Training**: Both models are trained using the preprocessed data, with hyperparameter tuning applied to maximize performance.
- **Model Evaluation**: The models are evaluated using metrics such as Mean Squared Error (MSE) and R-squared, ensuring high accuracy and reliability of the predictions.
- **Visualization**: Graphs and plots show the model’s performance, including error distribution, feature importance, and comparison between the predicted and actual ratings.

By leveraging these models, we aim to provide accurate and efficient predictions for movie audience ratings based on a variety of input features, enabling a deeper understanding of audience sentiment towards movies on Rotten Tomatoes.
