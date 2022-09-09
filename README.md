# Neural_Network_Charity_Analysis

## Overview of Analysis:
The purpose of this analysis is to determine if any specific applicant that will be funded by Alphabet Soup will be successful. We will be using neural network machine learning to determine this.

## Results:
### Data Processing
    - The 'target' variable for the model was the 'IS_SUCCESSFUL' column. 
    - The 'features' variables for the model were all other columns except the 'IS_SUCCESSFUL'
    - Variables we removed from the dataset were the 'EIN' and 'NAME' columns.
        - We also dropped the 'AFFILIATION' column in the optimized version.

### Compiling, Training, and Evaluating the Model
    - For the initial attempt we had the following data:
        - 2 hidden layers which comprised of 80 neurons for the first layer and 30 for the outer layer. 
        - The first two hidden layers used the 'relu' activation function and the outer layer used 'sigmoid'.
        - Our first performance results was 54% accuracy. It had a 2.1 loss.
    - For the second attempt (optimized version) we had the following data:
        - 2 hidden layers which comprised of 75 neurons for the first layer and 25 for the outer layer. 
        - The first two hidden layers used the 'relu' activation function and the outer layer used 'sigmoid'.
        - Other steps we took to improve the performance:
            - removed 'Affiliation' column.
            - removed any column that had null values.
            - increase the # of epochs from 30 to 50.
            - adjusted the number of counts for the buckets that were created.
        - Our first performance results was 63% accuracy. It had a .84 loss.
            - This is not the target performance but it was still improved by almost 10%.

## Summary:
In conclusion we were able to improve the overall score by 10% but there is still room to improve. If this were to be done again it may be helpful to use a random forst classifier. This could provide a more accurate model since you can adjust the number of estimators and tree depth. 
        

