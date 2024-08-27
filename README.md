# Project Overview:  
Built RF and XGB models to predict whether a NYC taxi cab rider will be a generous tipper. ("generous tippers" = who tip > 20%)  

Attributes:

VendorID  
tpep_pickup_datetime  
tpep_dropoff_datetime  
passenger_count  
trip_distance  
RatecodeID  
store_and_fwd_flag  
PULocationID  
DOLocationID  
payment_type  
fare_amount  
extra  
mta_tax    
tip_amount  
tolls_amount   
improvement_surcharge  
total_amount    

Model Performances:  

	model	precision	recall	F1	accuracy  
0 RF CV	0.674919	0.757312	0.713601	0.680233  
0	RF test	0.675297	0.779091	0.723490	0.686538  
0	XGB CV	0.673074	0.724487	0.697756	0.669669  
0	XGB test	0.675660	0.747978	0.709982	0.678349  

Key Insights:  
Yes, this is model performs acceptably. Its F1 score was 0.7235 and it had an overall accuracy of 0.6865. It correctly identified ~78% of the actual responders in the test set, which is 48% better than a random guess.  
It is interesting that VendorID is the most predictive feature. This seems to indicate that one of the two vendors tends to attract more generous customers.   


