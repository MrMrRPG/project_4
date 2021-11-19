# project_4_turochamp by pink + pandas.py

<a href="https://mrmrrpg.github.io/project_3/">Project_3_TuroChamp</a></br>

<b>Directory</b></br>
1. To access our dashboard: Please click on the link of Project_3_TuroChamp above
2. To observe our JS files: Please nagivate to the "static" folder
3. To access our Flask-based API: Please click on "app.py"
4. To acess our Supervised Machine Learning codes: Please navitage to the "Data_CSV" folder and click on "Starter_Code_not_dropped_columns.ipynb"

<b>Members</b></br>
Benji</br>
Meagan</br>
Josh</br>
Sam</br>

<b>Domain</b></br>
Applying Supervised Machine Learning in Chess

<b>Topic</b></br>
Chess

<b>Angle</b></br>
How to Predict Outcomes Based on First 3 Moves

<b>Methodology</b></br>
Using our primary dataset named "Games.csv" in our Resources folder, our team had access to over 20,000 records of chess games outcome data to train our machine learning algorhythm. In terms of data massaging, our team wanted to convert the column "Moves" which contains a sequence of the moves the particular player used in a single game. Using Excel, our team used "Text to Columns" to extract the moves and turned each move into individual columns (since we only wanted the first three moves per game to use for our prediction). Before the data is used, our last step was to drop unnecessary columns so there would not be so much noise. We dropped "id", "increment_code", "black_rating", "white_rating", "opening_name", "opening_ply", and "turns". Finally, now that our data is primed, we went ahead and split our data into training and testing sets with the column "winner" as our target data. Under the "winner" column, we have 3 possible outcomes: "black", "white", or "draw".<b></b></br>
Using Pandas, our team experimented with two particular methods of machine learning: Logistic Regression and Random Forest Classifier.

<b>Observations</b></br>
Using Logistic Regression yieled an accuracy score of 34%. We believe the low score is due to the fact that Logistic Regression is only meant to return a probablity value of 0 or 1. In our target data, we had up to 3 possible outcomes: black, white, or draw. Since having 3 possible outcomes in our target data seriously interfered with this model's learning, we had a poor result in accuracy. <b></b></br>
Moving onward, we applied the Random Forest Classifier on our existing training and testing dataset. Once again, with over 20,000 instances, we yieled an accuracy score of 93%. This is a significantly better score given that our group avoided overfitting by removing redundant features. Additionally, using Random Forest, the program was able to create multiple decision trees to influence its accuracy. An important consideration we had was our Feature Selection process. For prediction purposes, we wanted to carefully consider what data are highly relevant to predict the outcomes accurately. As mentioned above, a key feature we kept was the first 3 moves utilized in each game as we believed that the first 3 moves are highly critical in determining the outcome. We also kept the "rated" and "created_at" features as we also believed that they were key indicators. <b></b></br>
To test our numbers out to the next level, we simplified the possible outcomes by only keeping two values in our "winner" target column: black or white, with all rows having "draw" removed. Upon executing Logistic Regression, we yieled a 50% score which is an improvement, but still far from desirable. Upon using Random Forest Classifier with "draw" removed, we now have 97% testing score. 


<b>Possible Datasets</b></br>
<a href="https://www.kaggle.com/vikasojha98/top-women-chess-players">Top Women Chess Players</a></br>
<a href="https://www.kaggle.com/odartey/top-chess-players">Top 100 Chess Players Historical</a></br>
<a href="https://www.kaggle.com/datasnaek/chess">Chess Game Dataset (Lichess)</a></br>

<b>Possible APIs</b></br>
<a href="https://www.chess.com/news/view/published-data-api">Published-Data API</a></br>
<a href="https://lichess.org/api">Lichess API</a></br>

<b>Other Relevant Resources</b></br>
<a href="https://www.chess.com/members/titled-players/woman-grandmasters?&page=1">Woman Grandmasters (WGM) on Chess.com</a></br>
<a href="https://api.chess.com/pub/titled/WGM">JSON List of WGMs</a></br>

<b>Database</b></br>
Microsoft Azure

<b>New JS Library</b></br>
Google Charts

<b>Slides</b></br>
<a href="https://docs.google.com/presentation/d/1-GgaypWJtLD9YS8pDuaeQwrsGmZznVuhTCam62pIR6Q/edit?usp=sharing">Slide Deck</a></br>

<b>Bibliography</b></br>
<a href="https://www.titledopens.com/">Titled Chess</a></br>
<a href="https://github.com/gsfleur/titledopens">Titled Chess Github Repository</a></br>
<a href=https://github.com/StevenAdema/chess-opening-popularity>chess-opening-popularity</a></br>
<a href=https://python-chess.readthedocs.io/en/latest/>python-chess</a></br>

<img src="https://64.media.tumblr.com/f8e0a9a5b5a0f2fd5538d5a7bba1273f/tumblr_mqbflxsjRg1rn2sy0o1_500.gifv" alt="Panda Chess
by ~jmaaa">
