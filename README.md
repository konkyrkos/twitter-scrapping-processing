# twitter-scrapping-processing
This repository provides my solution for the 1st Assignment for the course of Practical Data Science for the MSc in Data Science at Athens University of Economics and Business.

## Scrapping Twitter Accounts

Connecting and fetching the 10 most trendy topics for Athens, Greece
Scraping 10 usernames from `https://www.businessinsider.com/uk-politics-twitter-accounts-2016-8?r=US&IR=T#48-matt-singh-2 containing the 49 best Twitter accounts to follow in UK politics putting them in a list

## Fetch Tweets

Scraping the Twitter accounts of all the UK parliament members and putting them in a DataFrame making sure that the followers_num is shown as a number, not a string.
Assessing the Party Tweeter Power with groupby() and using pandas' plot() and seaborn's barplot() to present this power.

## Processing Text Content

### Prepare profanity set

Using http://staffwww.dcs.shef.ac.uk/people/G.Gorrell/publications-materials/abuse-terms.txt as a source of abuse terms and discarding any noise.

### Parse tweets

Reading tweets from https://raw.githubusercontent.com/t-davidson/hate-speech-and-offensive-language/master/data/labeled_data.csv.
The class column specifies in which category the tweet belongs. A tweet can be classified into 3 categories: hate speech (class = 0), offensive language (class = 1) and neither (class = 2).
Creating a new column with the list of words of the each text, placed in a Python list.

### Count abuse term

Using the bad_words set you created in order to detect bad words in the word list of each tweet.
Saving the number of bad words found in each list in a new column.
Finding the mean, median, minimum, maximum, and sum of bad words in each class.

### Visualizing profanity
Creating plots presenting bad words per class.
