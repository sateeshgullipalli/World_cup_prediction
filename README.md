# World_cup_prediction
The goal of this project is to use machine learning to predict the winner of ICC T20 world cup planned to be held in October 2020.
## Data Description
The matches dataset has the information regarding the T20 matches played to date 29th January 2020 along with the results of the match, the date on which the match was played and the place of the match. There are a total of 1077 matches results.

![image](https://user-images.githubusercontent.com/62916741/94977268-ae17a200-04dd-11eb-89f7-4180a294194f.png)

The fixtures dataset has the information regarding the matches to be played in this world cup till the qualifiers, the details of the round and the date on which the game would be played. There a total of 42 records.

![image](https://user-images.githubusercontent.com/62916741/94977306-c982ad00-04dd-11eb-8026-40db9087f721.png)

The ground_countries dataset has the details regarding the country the ground belongs to, it is in the below format.

![image](https://user-images.githubusercontent.com/62916741/94977320-d6070580-04dd-11eb-88e6-d10ebd3f6264.png)

## Preprocessing Data
Although the data has no missing values, the Countries column has details of both playing teams in one column and the Result column has information regarding the winner along with the details of the win. These records were transformed to obtain playing teams in two different columns and the winner in the other column. Also, records that have no result has been dropped from the dataset.
The matches data set has details regarding the ground venue, we have joined this dataset with ground_countries dataset to fetch the country the match is played in. After performing the necessary steps, the dataset is now in the below format.
## Emperical Analysis
We have used Support vector machine algorithm with linear, radial and polynomial kernels and Random Forests models on our datasets to make predictions.
Our model is a supervised model and belongs to a classification task since the output is a categorical value. Input variables are the two teams participating in the match and the variable indicating if the team 1 is playing in its home ground. We have assigned 1 to the home ground column if team1 is Australia (Since Australia is the host country) else we assigned 0 to the home ground column. Our inputs are of the categorical data type. Hence, we used one-hot encoding to convert the categorical variables into the numerical format for the machine learning output. 
## Conclusion
After performing predictions on the qualifiers, Sri Lanka and Ireland remained at top 2 positions from Group A; Bangladesh and Namibia remained at the top 2 from Group B. These four teams advance to further rounds.
We further performed predictions on the super 12 matches, and we obtained the below results:
Australia and Pakistan remained at the top 2 positions from Group A.
India and England are at the top 2 positions from Group B.
When we performed further predictions on semifinals, India and Australia reached finals and India won against Australia in the finale.
We have obtained the predictions of all the matches in the upcoming world cup; by looking at the results a team can work on its performance and enhance their chances of winning the game as well
