# AI-in-QC
AI in Quality Control
This case is based on factory that produces steel plates in the final step of the production system
Our aim is to maximize the efficiency of the production system
We are trying to identify the possible types of steel plate faults (7 in total) only considering the metadata of the products.
With 1941 samples at our disposal, the distribution of the total faults is unbalanced in favor of ‘Other Faults’ class
We want to get immediately some results. So we take all our data and fit a Gradient Boosting.
We are able to achieve an overall ACCURACY of 0.807%.
Other_Faults is a noisy class because when we inspect a plate with a bump and a stain on the surface at the same time we put it in Other_Faults.
At this point, we try to make a model which not takes into account the Other_Faults class.
We fit a Gradient Boosting as above.
Now the ACCURACY is 0.909%, improving by 10 percentage points.
Credits to Marco Cerliani for this example
