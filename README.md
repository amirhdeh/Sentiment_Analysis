# Sentiment_Analysis
I used data mining to find about 50000 comments on digikala(a website like amazon in Farsi) and then labled the comment with a score more than 7/10 with possitive score 
and comments with score less than 3/10 with negative score.(I ignored the rest of the comment because they were mostly neutral).
Our goal is to determine wether a paragraph is considered positive or negative.

Foe embedding the vector I used a both a normal embedding which is lemmitizing each word and then transforming it to an integer based on our corpus and I also used a pre trained 
BERT engine for embedding.

For training I used a Bi directional LSTM cell with maximu of 100 words(cells) and then fed each paragraph to it. I also used a RNN system for comparison purposes.
The accuracy is 91% for the LSTM and the accuracy for negative comments is 97%.
