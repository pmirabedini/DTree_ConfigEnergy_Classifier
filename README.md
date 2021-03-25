# Decision Tree Classifier - Structure energy Correlation
In this code, I explored possible correlations between initial configuration of water molecule on a solid surface and the system's final energetic stability. 
This code uses a dataset of 5000 configurations of water molecule on a photocatalytic surface. I generated the data using molecular dynamics simulations. The data is not published. However, it can be provided under request and with my advisor's permission. 

## How does the code work?
Our goal is to define a classifier that can predict energy group of a molecule configuration on a slab surface.
steps to this end: 
1. **Initial data analysis:** check the features and how they relate to our target (energy).
2. **configuration space computation:** compute configurational space parameters.
3. **Kmeans clustering:** to find clusters of energy. 
4. **Second data analysis:** analyze the relation between configurational space and clusters of total energy. 
5. **Decision Tree Classifier:** Train and test a decision tree model. 

## Results 
for the data of water molecule on surface, the model provides good prediction of the two lowest energy groups, but a rather less accurate prediction for the other two energy groups, where the data is sparce. Note that in general, providing a good prediction for these data is a hard problem due to dealing with many configurations with similar energies. 

![Original vs. Prediction](/.images/Picture1.png?raw=true "Original vs. Predicted Energy Groups")