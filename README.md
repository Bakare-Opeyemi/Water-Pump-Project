# Water-Pump-Project
Predicting the remaining useful life of a water pump based on readings from 50 sensors strategically placed to measure the pump's parameters
## Data
The data contains readings from a set of 50 sensors monitoring a water pump and the corresponding remaining useful life of the water pump based on this readings, for each sample. The remaining useful life of the water pump is the target variable which will be predicted in this project. The original datset can be found here https://www.kaggle.com/anseldsouza/water-pump-sensor-data
## Analysis
Exploratory data analysis was first carried out on the dataset by computing the summary statistics and visualizing all available parameters at specific time intervals. Next we visualize the monthly and daily trends in the dataset. Doing this on the remaining useful life of the water pump;

![download](https://user-images.githubusercontent.com/64379963/154838802-d5672472-d1c4-4dbf-98ce-8b37e8dfa13e.png)

![download](https://user-images.githubusercontent.com/64379963/154838877-c113fd31-58c3-4a4b-b0c2-7d0ae7b29d60.png)

![download](https://user-images.githubusercontent.com/64379963/154838908-35611db1-9ece-42f4-b838-a525f6ecf2a4.png)

![download](https://user-images.githubusercontent.com/64379963/154838939-00846050-49bf-4250-bf06-4f59c69fa7bf.png)

The following major observations were derived from the dataset;
<ul>
  <li> The remaining useful life of the water pump steadily reduces after two months of continuous usage</li>
  <li> Daily aggregate changes trends show that the remaining useful life of the water pump only reduces with each passing day</li>
  <li> The remaining useful life of the water pump doesn't change much in the 4th month</li>
</ul> 

## Model Development
Eleven models were built on the dataset at first with the following results gotten;

![download](https://user-images.githubusercontent.com/64379963/154839671-4fbb07dc-5875-4f7d-ba0f-d5e382dfeeae.png)

![download](https://user-images.githubusercontent.com/64379963/154839687-5a0cd1cc-be34-4b3b-9f08-26b7b60ad937.png)

![download](https://user-images.githubusercontent.com/64379963/154839707-fb6870bc-28c7-41a2-9245-76bebf4e2a4e.png)

Using the results of model visualizations, and exploratory data analysis, feature engineering was used to reduce the dimensionality of the data set and help build more robust models. Ofcourse better results were arrived at

![download](https://user-images.githubusercontent.com/64379963/154839815-f3469a78-a565-46f4-a191-010797fca3fb.png)

#Conclusion
The kneighbors regressor algorithm performed the best on the dataset with an R2 score of 99.9% on training data and unseen data; mean absolute error of 1.004, Root meand squared error of 6.8 and a maximum error of 451.1

The model visualization also agrees with these results

![download](https://user-images.githubusercontent.com/64379963/154839929-412467d3-e9a4-4b0a-950e-75d3c21675c6.png)
