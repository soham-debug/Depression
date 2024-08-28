# Depression
In this project our aim is to help the depressed people who are using social media in their day-to-day life and express their emotions through their posts.
We begin by labeling Facebook data weekly, we collect the facebook data from by accessing token and the step given as follows: -

1.	Go to https://developers.facebook.com/docs/facebook-login/guides/access-tokens/
2.	Select Tools
3.	Select Graph API Explorer
4.	Login to facebook
5.	After login click on generate access token and select permission we want.
6.	After getting permission get access token and copy that access token to above token field
7.	After entering the token user get facebook post.

and then by analyzing the posts we pre-process the data by using natural language processing(NLP) that involves various techniques: -

a)	Stop Word Removal: - Which helps to remove the common words like “a”, “an”, “the”, “is”, “an”, etc.,
b)	Stemming: - Words are reduced to their base form i.e., from stressed to stress and happiness to happy, etc.
c)	POS tagging: - POS tagging helps in extracting meaningful keywords that indicate emotions or mental states. Words tagged as adjectives (like "tired") or verbs (like "can't sleep") are more relevant for understanding emotions than prepositions or articles (like "at," "the").
d)	Keyword Extraction: - Important words like "awesome," "stressed," "hopeless" are identified because they indicate mood.

Then after extracting the keywords sentiment analysis is used to classify the negative and positive words and a neutral.
To determine whether a user is depressed, we use Long Short-Term Memory (LSTM) networks combined with the Swish activation function. 
LSTM reads a sequence of posts from a user, one after the other, and tries to understand how the user’s mood is changing over time. The LSTM is really good at remembering past information, so it can connect what was said in earlier posts with what is being said now.
The Swish activation function is like a booster for the LSTM. It helps the LSTM better understand and learn the patterns in the posts. Swish makes the LSTM more sensitive to small changes in the posts, which helps it pick up on subtle shifts in mood that might indicate a growing problem, like increasing stress or depression.
