# **Ada Project : Creative extension**
## Milestone P3

### **Supplementary method :** Decision tree

2. Abstract:

The idea of the original paper is to demonstrate (if possible) that there is a racial profiling trend across the united states, the authors do so by using several methods that mostly take data across all available states. We would like to limit the search to one state, as we think that there may be different trends in the different states (As demonstrated for instance by the marijuana legalisation/search rate test). Moreover our choice to limit ourselves to one state is also driven by the fact that most states don't have the data we require. We also want to implement a method that the paper hasn't used: the decision tree, which we think is a robust statistical test that corresponds to the data we have and that will enable us to assess the statistical importance of each of the variables a police officer may take into account. We know that our conclusions only apply to the specifical instance of the washington state patrol, but that is the aim. 

3.	Research Questions:

We want to find out which variables affect the outcome (search or no search) the most. The variables that we are interested in are perceived race, age, sex, state of the legalization and the years since the change in legalization. We will also be interested in the precision, accuracy and recall of the predictions and we will try to tune the parameters available to us (we will explain this in methods) so that we can have a valid prediction. We are also interested in what could affect that accuracy without our methods showing it. In fact we suspect as the authors of the paper do, that some information may have been withheld and we will therefore try to assess how much data we had to filter out and what impact it could have on our analysis.

4.	Proposed dataset:

The original paper gives a link to the source of their data the Stanford Open Policing project :https://openpolicing.stanford.edu/data/. Severall million of stops are categorized there but as we said we decided to limit ourselves to only one state, which we thought needed to be heavily populated and where state patrols had recorded  a lot of stops with information on the racial appearance of the subjects, the time of the stop, the subject age, the subjet sex and if a search had been conducted. Our choice is therefore the state of washington and the 11 million state patrol stops, which we think is appropriate for our needs.But this also means that the file containing all these stops is really large and as we have already experimented it takes a little moment to load everything and to handle it afterwards, this problem is solved by removing all the stops that don't have the neccesary data and by removing the information we don't need. We will maybe create a cleaned csv from which we will work so that we don't have to load and do the filtering each time we open the notebook.
Moreover if the decision tree works as we expect we want to be able to compare the decision trees from different states so we wil maybe repeat the filtering procedure on another dataset that has the appropriate information.

5.	Methods:

We will perform a Decision Tree Analysis on the stops of the washington state police, with the help of the sklearn library. We will then compare the accuracy, precision and recall between the different models with the SGD classifier, logistic regression and random forest. We also perform an optimization based on validation set precision (Grid search cross validation).

 We will also reproduce our optimized tree on different states and calculate missing data ratios.

6.	Proposed timeline:

 We have already done some tests and loaded the data. We will be done with a first tuned tree for washington state patrols in the course of the next week. We will then be able to adjust what will need to be adjusted and we will have a week or so to perfect our methods and begin implementing it for other states. We will be able to visualize all of our analysis and draw the appropriate conclusions. The remaining time will be used to replicate the rest of the paper and correct possible mistakes of our extension.

7.	Organization within the team:

p4.1 Finish the first Tree

p4.2 Replicate the methods for other states and compare results

p4.3 Visualization of everything and Conclusions

p4.4 Replicate paper

8. Questions for TAs (optional):




