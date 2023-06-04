# Retrieve-tweets
Retrieve the most recent tweets of a specified Twitter user 

The code is a Python script that uses the Tweepy library to retrieve the most recent tweets of a specified Twitter user and stores them in a CSV file.
The code requires the user to replace the placeholder values for consumer_key, consumer_secret, access_key, and access_secret with their own Twitter API credentials. These credentials are necessary to authenticate and authorize the script to access the Twitter API.

The main function of the code is get_tweets, which takes a Twitter username as input. It initializes the Tweepy OAuthHandler with the provided credentials and sets the access token. Then, it creates an instance of the Tweepy API using the authenticated credentials.The variable number_of_tweets is set to 100, indicating that the script will retrieve the 100 most recent tweets from the specified user.

The code uses a for loop with the Tweepy Cursor to iterate through the user's timeline and retrieve the desired number of tweets. Each tweet's information, including the username, tweet ID, creation timestamp, and text, is stored in a list called tweets_for_csv.Finally, the code creates a CSV file with the username followed by "_labwork.csv" as the filename. It writes the collected tweet data to the CSV file using the csv.writer. The CSV file will have columns for the username, tweet ID, creation timestamp, and the text of the tweet.

To run the script, the user needs to provide the Twitter username as a command-line argument when executing the script. If the script is run with more or less than two arguments (including the script name itself), an error message will be displayed.The output of the script is the creation of a CSV file containing the specified user's most recent tweets, with each tweet's relevant information in separate columns. Additionally, the script prints a message indicating the name of the CSV file that was created.
