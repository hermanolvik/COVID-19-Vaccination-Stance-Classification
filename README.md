## COVID-19 Vaccination Stance Classification

This is a machine learning project aimed at implementing a classifier for determining the stance of social media comments towards COVID-19 vaccination, achieving 90% accuracy and providing insights into public sentiment. The project is implemented in Python using the scikit-learn library. The goal of this project is to classify social media comments as either pro-vaccination or anti-vaccination. The classification model is trained using a dataset of annotated comments collected and labeled by multiple reviewers.

### Dataset

- **Source**: Comments were gathered from various online platforms by students at Chalmers University.
- **Annotations**: Each comment was labeled as pro-vaccination, anti-vaccination, or neutral. A majority voting system was used to determine the final labels.
- **Final Dataset**: The dataset includes comments labeled based on majority votes, with ties discarded.
- **Text Preprocessing**: Comments were standardized to lowercase, punctuation was removed, and they were converted into TF-IDF vectors.
- **Split**: The first sample was split into training (80%) and testing (20%) sets for initial model evaluation.

### Models Implemented

Various machine learning models from the scikit-learn library were used to train the classifier:

- Logistic Regression
- Support Vector Classifier (SVC)
- Random Forest Classifier (RFC)
- Gradient Boosting Classifier (GBC)
- Neural Network Classifier (NNC)

Hyperparameter tuning was performed using GridSearchCV to optimize model performance.

### Key Findings

- **Best Model**: The Support Vector Classifier (SVC) with hyperparameters C=10, gamma=1, kernel='rbf' achieved the highest accuracy of 90%.
- **Feature Importance**: The logistic regression model highlighted key features, such as the term "antivaxxers," which strongly predicted a pro-vaccination stance.
- **Consensus Analysis**: The average consensus score for the final dataset was 0.9966, indicating high agreement among annotators.

### Limitations

- **Time Constraints**: The project was completed within a one-week timeframe, limiting the scope of model exploration and data processing techniques.
- **Complexity of Models**: The project focused on models available within the scikit-learn library, excluding more complex methods like BERT due to resource and time limitations.

### Future Work

Future research could explore alternative feature representations and fine-tune additional models to further enhance predictive accuracy.

### Contact

- Herman Olvik: olvik@chalmers.se
- Cornelia Swartling: corswa@chalmers.se
