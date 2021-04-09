# Diffuse-Large-B-Cell-Lymphomas-Prediction
DLBCL is the most common subtype of non-Hodgkin lymphoma (NHL), globally constituting up to 40% of all cases [3]. 
In the US alone, out of 100000 people, it affects about seven of them every year. It is fast-growing and is a very aggressive form of NHL. 
It is fatal if left untreated, but with appropriate treatment at the correct time, near about two-thirds of them can be cured.

The dataset used in this project is DLBCL dataset. Link: https://file.biolab.si/biolab/supp/bi-cancer/projections/info/DLBCL.html

This particular dataset has as many as 7070 attributes but only 77 instances. Since, the no of attributes is large, 
analysis of this kind of dataset becomes difficult for the doctor as well as automatic diagnosis process through computing devices becomes complex and time-consuming.
This is why we need feature selection.

Here, an ensemble of 3 feature selection methods have been applied to increase accuracy.

As a part of preprocessing, values of both the datasets have been standardized and then normalized.
After the preprocessing, three ML algorithms RNF, KNN and NB have been applied on the datasets with 10-fold cross validation and accuracies have been noted.
A union of the top n features obtained from each filter method has been considered. 
Then on the reduced feature set identified as important features, the classifier have been applied.

The outcomes obtained from our work have successfully met the objectives of maximizing predictive performance, 
including all the prime features which a single filter method might have missed but at the same time also removing the redundant features. 
The least ranked features by the ensemble are the ones which have least importance in the dataset in terms of information, dependence as well as distance. 
This ensemble has been coined the term "MIRFCS".
Thus, MIRFCS also provides the information about the noisy, redundant or unnecessary features which are then discarded. 
Furthermore, selection of best set of features reduces the time consumed for analysis. 
All the three diseases which have been studied in this work are incurable but if diagnosed in time, can be controlled. 
This system can do that with the diagnosis time being minimum, treatment starting at the earliest, lesser attributes meaning lesser tests, 
hence economically benefiting for the patients.
