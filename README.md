🏏 IPL Match Winner Prediction

This project is centered around building a machine learning-based system that can predict the winner of IPL matches with a fair degree of accuracy. The core idea is to make use of historical IPL data, which includes not only the final results of past games but also rich information such as team performances, player contributions, match conditions, and ball-by-ball events. By processing and analyzing this data, the model is able to identify key patterns and trends that typically influence the outcome of a match.

The system takes into account crucial in-game factors like the current score, wickets remaining, overs left, and required run rate, and combines them with past performance metrics of teams and players. Using this information, the model calculates real-time probabilities and offers predictions about which team is more likely to win as the match progresses.

📂 Files & Folders

├── app.py              # Streamlit application (UI for predictions)  
├── data.ipynb          # Notebook for data cleaning & EDA  
├── model.py            # Code for model training & testing  
├── dataset.csv         # Dataset used for building the model  
├── requirements.txt    # Python libraries required  

⚙️ Setup

Clone this repository:

git clone https://github.com/YourUsername/IPL-prediction.git
cd IPL-prediction

Install dependencies:

pip install -r requirements.txt

🚀 How to Run

Start the Streamlit app with:
streamlit run app.py


Once running, open the browser at:
👉 http://localhost:5000

📊 Data Workflow

Loading the Data
Uses matches.csv and deliveries.csv as input.
Cleaning & Preprocessing
Combines match-level and ball-by-ball data.
Removes D/L affected matches (dl_applied = 0).
Keeps only useful columns and renames them for readability.
Feature Engineering

Some of the features created are:

current_score → Runs scored so far.
runs_left → Remaining runs to chase.
balls_left → Balls left in the innings.
wickets → Remaining wickets.
crr → Current run rate.
rrr → Required run rate.

🤖 Machine Learning Model

Algorithm used: Logistic Regression
Trained on engineered features.
Performance checked using accuracy metrics.

📈 Match Insights

The project also includes simple visualizations to track:
Runs progression
Wickets over time
Predicted win probability

🤝 Contributions

Want to improve this project? Feel free to fork it, raise issues, or submit PRs.

📜 License

This project is released under the MIT License.
