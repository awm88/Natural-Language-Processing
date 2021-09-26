# Natural-Language-Processing
The first NLP project is webscrapping reviews from TrustPilot. The file is 'TD_official_final_assignment_pynb (4).ipynb'
The steps are as follows:
1. Use the requests module to download the html for URL.
2. Extract the total number of reviews. For example the Skype page: <h2 class="headline">Reviews&nbsp;&nbsp;<span
class="headline__review-count">1,292</span></h2>
3. Iterate over the review pages.
Example:
Python for i in range(num_pages): page = requests.get(URL + '?page=' + str(i + 1))
4. From each page extract the reviews.
5. From each review, store the following to the CSV file:
comapnyName, e.g. Skype.
datePublished, the date when the review was published.
ratingValue, the the numerical value of the rating.
reviewBody, the review text.
6. The final CSV file should have at least 500 rows and four columns ("comapnyName", "datePublished", "ratingValue", and
"reviewBody").

The second NLP project is Sentiment Analysis where I built a sentiment classifer to classify reviews. The file is 'nlp_assignment_2 (1) (2).py'
My task is to do sentiment analysis of the reviews by training and testing a BoW text classifier on the review
texts using RatingValue as labels. The ratings are binned into negative (ratings 1 & 2 ), neutral (rating 3 ) and positive
(ratings 4 & 5 ) sentiment. The binned ratings are coded with negative as 0 , neutral as 1 and positive as 2. My code does the following:
loads the reviews.csv , preprocesses the data, splits it and saves the files as training.csv and valid.csv, loads training.csv and trains the model, and loads the validation data ( valid.csv ) and prints the performance metrics on the validation set.

The third NLP project which is 'final100' is sentiment analysis with a neural language model. The file is 'final100 (1).py'
