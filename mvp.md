# Analysis of features of film and their correlation with the lifetime worldwide gross


As the idea for this project is to determine which films would be profitable in the long term, our goal is to predict the lifetime worldwide gross, by analyzing
the features of the films and finding which of those hold a higher correlation with our prediction target. 


After gathering all of the data, we found that the variables that hold a higher correlation with the target are:

<img width="700" alt="Screen Shot 2021-09-28 at 5 28 53 PM" src="https://user-images.githubusercontent.com/34829066/135169059-befa2ab3-81f1-459c-a259-08e9ecd76712.png">

- Domestic Opening
- Domestic Lifetime Gross (we won't use this feature because if our purpose is to predict, we won't have access to this information)
- Budget 

Then, we can see the relation between the features and the target by using pairplot from Seaborn. 

<img width="779" alt="Screen Shot 2021-09-28 at 5 28 43 PM" src="https://user-images.githubusercontent.com/34829066/135169020-d345db56-9843-43b6-aa3a-96a5ec7c872f.png">


For now, we have build a simple training/validation/test model 

<img width="1096" alt="Screen Shot 2021-09-28 at 5 46 57 PM" src="https://user-images.githubusercontent.com/34829066/135170355-e53013d1-de83-4850-8525-8f546f4b8fa1.png">


The end goal with the project, will be to create dummy variable out of the genre and the distributor company, to see if any of those features
will hold a high correlation with the worldwide gross. 

