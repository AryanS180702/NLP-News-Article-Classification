# News Article Classification

## Dataset

🔗 [News Article Dataset](https://docs.google.com/spreadsheets/d/1m4YMfqQxo_DcbtzGqbfZitvJmytbWUE8qjixhHmtadk/edit?usp=sharing)

It contains:
- **Total entries**: 50,000 articles
- **Target variable**: `Category`
- **Input features**: `Headline`, `Short Description`, and `Keywords`

## Steps Taken

1. **Importing the Dataset**  
   - Loaded and previewed the dataset

2. **Data Cleaning**  
   - Checked for null values and handled them appropriately  
   - Dropped unnecessary or irrelevant columns

3. **Data Preprocessing**  
   - Removed HTML tags, punctuation, and extra whitespace  
   - Converted text to lowercase  
   - Combined headline, short description, and keywords into a single text field

4. **Exploratory Data Analysis (EDA)**  
   - Analyzed class distribution  
   - Explored text length across categories  
   - Identified top words per category  
   - Created word clouds to visualize common terms

5. **Feature Extraction**  
   - Tokenized the combined text  
   - Removed stopwords and applied lemmatization  
   - Split the data into training and test sets  
   - Applied TF-IDF vectorization to convert text to numerical features

6. **Model Development**  
   - Trained four different models:
     - Logistic Regression  
     - Naive Bayes  
     - Random Forest  
     - Support Vector Machine (SVM)

7. **Model Evaluation**  
   - Evaluated all models using classification reports and confusion matrix heatmaps  
   - Compared accuracy and F1 scores across models using visual bar charts

8. **Model Selection**  
   - **Logistic Regression** was selected as the final model due to its superior performance  
   - **Accuracy**: 0.81  
   - **F1 Score**: 0.81

9. **Prediction Class**  
   - Built a class that takes in a headline, short description, and keywords  
   - Performs preprocessing and vectorization  
   - Uses the trained model to return the predicted category of the article

## Results

The Logistic Regression model performed the best among all tested algorithms, achieving:

- **Accuracy**: 0.81  
- **F1 Score**: 0.81

The model is effective in classifying articles into appropriate categories, making it a useful tool for content tagging and recommendation systems.
