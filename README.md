# charity_funding_predictor
This is my solution to homework 21 for data bootcamp. Click on the Analysis for images. Dom said we could skip the callback that save epochs step.


## Overview:
Alphabet Soup is a nonprofit foundation looking for a tool for selecting applicants for funding. The tool's purpose is to create an increased chance of better-funded ventures. I set myself with the goal of having 75% accuracy in predicting the chance of a venture being successful under Alphabet Soup. Alphabet Soup sent me a CSV with data from 34,000 organizations that they have funded. I used this CSV as I created a neural network to create the tool.

<br>

## Results:
<br>

### Data Preprocessing
<br>

The target for my model was the column “Is_Successful”. I chose this as my target variable because it is the output I am looking to predict with my model, is the organization successful or not.

The features for my model are the columns, "Application_Type, Affiliation, Classification, Use_Case, Organization, Status, Income_Amt, Special_Considerations,  and Ask_AMT.” All of these columns play some part in predicting if an organization will be successful.

I got rid of the columns, “EIN, and Name”. These columns were not going to have an effect on the outcome of an organization were just creating noise so it is best to remove them.

<br>

### Compiling, Training, and Evaluating the Model
<br>

I created three models to attempt to reach my goal of 75%. In my first model I used two hidden layers, the first had 80 neurons and the second had 30 neurons. I chose to use “relu” as my activation function and 50 EPOCHS. This gave me 72.89%. 


In my second model, I added a third hidden layer, the first had 90 neurons, the second had 30 neurons, and the third had 30 neurons. I kept “relu” as my activation function and 50 EPOCHS. This did not change my percentage as I was still at 72.89%.


In my third model, I added a fourth hidden layer, the first had 90 neurons, the second had 60 neurons, the third had 30 neurons, and the fourth had 10 neurons. I once again kept “relu” as my activation function and used 50 EPOCHS. Once again I had only slight improvement with a 72.97%.  

<br>

## Summary:
After all three models, I was only able to reach 72.8% accuracy, which is lower than the goal of 75%. It is possible to increase the accuracy by changing some other features, how many neurons are in a hidden layer, the number of hidden layers, the activation function used, etc... From my experience adjusting these factors only played a minor factor in the accuracy of the model. It is because of this I would recommend using a different model to predict whether it would be a successful venture for Alphabet Soup to fund an organization.
