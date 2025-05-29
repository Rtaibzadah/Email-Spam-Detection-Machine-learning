# Email-Spam-Detection-Machine-learning

Spam Detection
Introduction
This first task, spam detection, is about creating a model that can tell if a message is a spam message or not. There's 2 sets of data — one of them is the training set, which includes both messages and a label variable (0 or 1) that shows if it's spam or not, and a separate test set.

Most of the code was already implemented in the template file. This included downloading the data, loading it, extracting the text and the labels from the training set, and the text from the test set. It also allowed for displaying text based on its label. (I didn't include the confusion matrix as I ran out of time.)

Methodology
I used TF-IDF to turn the messages into numbers so that the model can understand the text. In short, the model gives each word a number that helps with processing the data.

After that, I trained the logistic regression model and then used it to make predictions on the test messages.

Results

Above are some examples of the results. Due to the length of some outputs, I couldn’t include more examples.

After training the model, I ran predictions on the test dataset. Since the test data doesn’t come with any labels, I had to manually look through the predicted outputs to see if the model’s guesses made sense.

Below are some actual examples of messages with the model’s predicted label:

Some messages looked very corporate or business-related, like energy reports, meeting notes, or pricing details. The model mostly predicted these as not spam, which I agree with.

One message was motivational and kind of generic — the model predicted it as spam, which makes sense because spam messages often use that tone.

Most messages that mentioned contracts, volumes, attachments (like Excel files), or internal communication were all marked not spam, which again seems correct.

From what I could see, the model did well at telling the difference between casual or marketing-style spam vs. formal business messages. I didn’t find any major examples where I strongly disagreed with the model’s prediction.

