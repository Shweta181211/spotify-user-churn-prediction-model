## PREDICTING SPOTIFY USER CHURN USING LISTENING BEHAVIOR DATA ##
- This project predicts whether a Spotify user is likely to leave (churn) or stay based on their listening behavior and account details.

- Using machine learning (Random Forest Classifier) and a Gradio web interface, it allows anyone to input user details and instantly get a churn prediction.

## FEATURES ##
- Reads data from a Kaggle CSV dataset
- Processes & cleans data (encoding, scaling, splitting)
- Trains a Random Forest model for churn prediction
- Saves model, scaler & feature names for future predictions
- Provides an interactive Gradio web app to test predictions

## TECH STACK ##
1. Data Handling & Preprocessing
- Pandas: For loading and cleaning the dataset
- NumPy: For numerical computations

2. Machine Learning
- Scikit‑Learn: For preprocessing (StandardScaler) & model training (Random Forest Classifier)
- Joblib: To save and load the trained model, scaler, and feature names

3. Interface & Deployment
- Gradio: For building an interactive web app to make predictions
- Google Colab: Easy execution & sharing of the app

4. Dataset Source
- Kaggle → Spotify user churn dataset

## INPUT FIELDS ON WEB INTERFACE ##
- Subscription Type: Free, Premium, or Family
- Country: User’s country (e.g., India, USA)
- Avg Daily Minutes: Average daily listening time
- Number of Playlists: Total playlists created by the user
- Top Genre: User’s most-listened genre (e.g., Pop, Rock)
- Skips per Day: Average skips per day
- Support Tickets: Tickets raised to Spotify support
- Days Since Last Login: Inactivity duration

## EXAMPLE PREDICTION ##
- Input:
Subscription Type: Free
Country: India
Avg Daily Minutes: 45
Number of Playlists: 5
Top Genre: Pop
Skips per Day: 2
Support Tickets: 0
Days Since Last Login: 5

- Output:
Will probably stay (Chance: 73.40%)

## HOW TO RUN ON GOOGLE COLAB? ##
1. Open your Google Colab Notebook.
2. Copy and Paste the project code we have provided. 
3. Load the dataset we have provided. 
4. Run the cell- wait for a Gradio link.
5. Click the link- you will see a form to enter user details.
6. Fill details and Click Predict- see if the user will churn or stay.

## FUTURE IMPROVEMENTS ##
- Add more ML models (XGBoost, LightGBM) for comparison.
- Deploy on Hugging Face Spaces or Streamlit Cloud.
- Improve UI with dropdowns for categorical inputs.



