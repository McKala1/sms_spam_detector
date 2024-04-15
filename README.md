# sms_spam_detector
# Hello There! 🩷

Welcome to my SMS Spam Detector project! I'm so excited to share my work with you! 🌟 In this project, I've refactored code into a fabulous linear Support Vector Classification (SVC) model. Once the model was trained, I created a Gradio app that lets users play around with text messages to see if they're spam or not! How exciting! 📲

## Background 🌸

In this project, I've taken an SMS text classification solution and transformed it into a handy function that creates a linear Support Vector Classification (SVC) model! Once the model was set up and trained, I whipped up a Gradio app to host my fab application so users can test out text messages! The app gives feedback, letting users know if the message is spam or not based on how the model performs! 💌

## Files 💖

Here's a list of the files I used for this project:

- `gradio_sms_text_classification.ipynb`
- `sms_text_classification_solution.ipynb`
- `SMSSpamCollection.csv`

## Instructions 🌟

### SMS Classification Function 🌷

Here's how I created the `sms_classification` function using `sms_text_classification_solution.ipynb`:

- I set the features variable to the DataFrame's text message column.
- The target variable was set to the "label" column.
- I split the data into training and testing sets, setting the test size to 33%.
- I built a pipeline to transform the test set for comparison with the training set.
- After fitting the model to the transformed training data, I returned the model.
- I loaded the `SMSSpamCollection.csv` into a DataFrame and called the `sms_classification` function with the DataFrame, storing the result in the `text_clf` variable.

### SMS Prediction Function 💌

Next, I created the `sms_prediction` function to predict the classification of a new text message:

- I created a variable to hold the prediction of a new text message.
- I used a conditional statement to determine whether the text message is "ham" (not spam) or "spam".
- If the message was "ham", the function returned: `f'The text message: "{text}", is not spam.'`
- If the message was "spam", the function returned: `f'The text message: "{text}", is spam.'`

### Gradio Interface Application 💕

Finally, I brought my cute little Gradio app to life:

- I set up a Gradio Interface application with a textbox for input and a textbox for output.
- I added labels to each textbox to explain what they contain.
- I launched my adorable app, and now everyone can try it out!

**Testing**:
I've tested my SMS prediction Gradio app with these text messages:

1. "You are a lucky winner of $5000!"
2. "You won 2 free tickets to the Super Bowl."
3. "You won 2 free tickets to the Super Bowl. Text us to claim your prize."
4. "Thanks for registering. Text 4343 to receive free updates on Medicare."

I've had so much fun creating this SMS Spam Detector, and I hope you enjoy it as much as I do! 🌈




**References**
Tiago, A., Hidalgo, J. 2012. SMS Spam Collection. UCI Machine Learning Repository. Available https://archive.ics.uci.edu/dataset/228/sms+spam+collectionLinks to an external site. [2023, October 25]. (CC-BY 4.0Links to an external site.).
