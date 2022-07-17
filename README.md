# Neural_Network_Charity_Analysis
### Overview of the analysis:
The purpose of this analysis was to use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The analysis included a dataset of more that 34,000 organizations that had received funding in previous years. 
### Results: 
#### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
    The target is the "IS_SUCCESSFUL" column to determine whether a project that received funding is likely to be successful or not. 
    
- What variable(s) are considered to be the features for your model?
 Features include the other columns: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE,  ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS 	, ASK_AMT
- What variable(s) are neither targets nor features, and should be removed from the input data?
  The EIN and Name variable could be dropped from the input data. In later tests I also removed the 'STATUS' and 'SPECIAL_CONSIDERATIONS' variables as they had few unique variables. 
#### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  ![image](https://user-images.githubusercontent.com/100727593/179410839-ef5e9487-2fed-4bad-8677-62ab4741d8a6.png)

- Were you able to achieve the target model performance? No, the highest performance I was able to get was .73
 ![image](https://user-images.githubusercontent.com/100727593/179405484-cac110cc-a878-408f-b54f-678cd46705c8.png)

- What steps did you take to try and increase model performance?
I removed additional features that had limited unique variables- STATUS and SPECIAL_CONSIDERATIONS. I first tried to increase the number of neurons in my existing 2 layers and then when that didn't work I added an additional hidden layer. None of the changes resulted in a substantial improvement in accuracy.
