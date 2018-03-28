Will explore 2000 movie reviews and create an embedding and CNN, deep learning model that will predict if the sentiment of a movie review is positive or negative. This model could be beneficial for movie review sites to help give them an idea if a review is positive or negative.

	The data has been presented in two folders of which one folder being labeled pos and the other neg. Each folder has 1000 separate text documents. The positive reviews are in the pos folder and the negative reviews in the neg folder. I had to clean the text data by creating a function that does the following to the text data:
	
	1) Split tokens on white space.
	2) Remove all punctuation from words.
	3) Remove all words that are not purely comprised of alphabetical characters.
	4) Remove all words that are known stop words.
	5) Remove all words that have a length ≤ 1 character.
	
I also decided to remove words that did not hit the minimum threshold of occurring at least two times within all the documents of the respective folders. If a word only appears one time out of all 1000 documents, it was not included.

At this moment I’m not too sure what other datasets I could use with this project. Perhaps if I knew more about each review, such as something about the critic giving the review (gender, age, place of residence, etc) or when the review was given to add some sort of time series element to this project.

I used a 90/10 training/test split to create an embedding and CNN, deep learning model. My model provided 100% accuracy on the training set and 86.00% accuracy on the test set. I tested the model by inputting text "Everyone will enjoy this amazing film. It was so exciting and thrilling. I love it, recommended! Thumbs up!". The model predicted sentiment positive: 52.124%. I also tested the model by inputting text "This is a bad movie. Do not watch it. It sucks. Put me to sleep. Boring". The model predicted sentiment negative: 66.410%


