# Neural Network Charity Analysis
_________________________________
- We were given a CSV file  CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. 
### Purpose of the Analysis
*We were given a CSV file  CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. For this analysis we were already provided with a dataset that had features. For further analysis we were asked to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.*

### Results
*What variable(s) are considered the target(s) for your model?*
- Since we were to determine if the money was used successfully or not, our target variable was IS_Successsful column.

*What variable(s) are considered to be the features for your model?*
- For our X we chose to go with the other columns in the dataset as our input. We determined certain columns that were unnecessary for our data analysis and we removed them from the dataframe.

*What variable(s) are neither targets nor features, and should be removed from the input data?
- After removing the EIN & the NAME column we then had to do some further aternating to fit our data needs. Binning was one of the routes that we had to take. After determining the limit of the Unique values for APPLICATION_TYPE and CLASSIFICATION columns,  we created a for loop that would take in an arguement and name the unwanted values as "Other." Like the image shown below:

 ![mod19](https://github.com/mckenziekkilburn/Neural_Network_Charity_Analysis/blob/master/images/mod19.PNG)
 

*How many neurons, layers, and activation functions did you select for your neural network model, and why?
- For my original model, I chose to go with my input features the len of what X_trained scaled was and for my hidden layer 1 I chose 80 and the second layer 30. For the activation functions I chose ReLu for the input layers and Segmoid for the output layers. In the picture below it shows my original model before doing any editing. 

 ![mod19.1](https://github.com/mckenziekkilburn/Neural_Network_Charity_Analysis/blob/master/images/mod19.1.PNG)
 
*Were you able to achieve the target model performance?
- No I was not, after trying numerous approaches I could not get the models accuracy above 75%
*What steps did you take to try and increase model performance?
- I tried a number of things to try to increase the accuracy of my neural model. One being increasing the number of nodes of the model on each hidden layer. Another being adding an addition hidden layer, which did not improve my model. Also adding additional epochs for the model to take in. After messing with the callback and epochs funtions this is what helped my model the most and reached a 66% accuracy.

### Summary 
- In conclusion I got my deep learning model up to 66% which is not that great. I do think if I have more time I will be looking at this model again to see maybe where I went wrong with it. I did try out the Random Forest Classifier and it got a higher accuracy score that my deep learning model did. 
