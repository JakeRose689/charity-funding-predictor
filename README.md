# charity-funding-predictor

### Step 4: Write a Report on the Neural Network Model

For this part of the Challenge, you’ll write a report on the performance of the deep learning model you created for AlphabetSoup.

The report should contain the following:

1. **Overview** of the analysis: 
  * The non-profit foundation Alphabet Soup wants to create an algorithm to predict whether or not applicants for funding will be successful. 
  * This analysis will provide a reflection on my process and results developing this deep learning model for Alphabet Soup.

2. **Results**: Using bulleted lists and images to support your answers, address the following questions.

  * Data Preprocessing
    * What variable(s) are considered the target(s) for your model?
	* The target was simply the "IS_SUCCESSFUL" column, which let us know if the organization was successful or not.
    * What variable(s) are considered to be the features for your model?
	* The features were all other columns present in the dataset, save for two, which will be listed below.
    * What variable(s) are neither targets nor features, and should be removed from the input data?
	* The columns "EIN" and "NAME" were neither targets nor features and were both removed from the dataset.
  * Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
	* I iterated through three different attempts to create a model that would predict with greater than 75% accuracy, but was unable to do so. In the 3rd attempt, I started with 2 neurons in the input layer, 50 in the 1st hidden layer, and 25 in the second hidden layer, with one as the final output of YES or NO for success.
    * Were you able to achieve the target model performance?
	* My best model performance was just over 70% accuracy. The target was 75%, so I was unable to meet this goal.
    * What steps did you take to try and increase model performance?
	* I performed dimensionality reduction with PCA and t-SNE to try and quiet down any noise present in the model, and also adjusted the number of neurons in the hidden layers and their activation functions. These efforts improved model performance marginally, but not enough to cross the 75% threshold.

3. **Summary**: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

  * The overall results of the deep learning model were not altogether disappointing, as I was able to get accuracy over 70% in the testing dataset. I would be interested to see how a random forest classifier or a logistic regression would perform with this data. I feel like starting with a more simple model first is always the best way to go, then if they fail, continue to try more and more complicated models through each iteration. Starting off the bat with a neural network would not be my approach to attempting to solve this problem in the real world.
- - -