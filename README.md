# Global Terrorism Database

The Global Terrorism Database (GTD) includes information on 180k terrorist attacks, from 1970 through 2017.
For most of the attacks, the terror group that carried them out is identified. 
I have predicted the terror groups responsible for the terror attacks whose perpetrator is unknown.


I have used the Random Forest model. RF can be efficiently used with large datasets and can handle high-dimensional data. An additional "bonus" is that RF is highly economical in terms of preprocessing, handling both categorical and numerical variables. 

RF identifies the features with the largest contribution to the model. I used this to save computing time, running the model on a subset of the data first, and selected the most contributing features to be used for the sake of further exploration.  

The chosen metric of success was an intuitive one - the hit ratio (the number of times that a correct prediciton has been made divided by  the total number of predictions). The hit-ratio for the validation set was 82.03% .

To be added : 
* A more systematic search for the model hyper-parameters (grid search)
* k-fold cross-validation
