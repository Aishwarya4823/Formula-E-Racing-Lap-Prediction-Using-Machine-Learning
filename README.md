## Formula E-Racing Lap Prediction Using Machine Learning<br>
Formula E Racing is the world’s first full electric, international one-seater, street racing championship. Apart from bringing awareness to fighting climate change, it is also creating a technological and sustainable development test bed that helps address mobility and other environmental issues. Furthermore, it is the first global sport with net zero carbon footprint. 
<br><br>
The prediction question that we have tried to answer is if, using historical data, we can predict the number of laps the driver will need to complete the race. <br><br>
The reason why it's important to solve this business case is because once a driver would know how many laps are left in a race, then that would help him better frame his energy optimization strategy.<br><br>
For example, if our model predicts that the number of laps remaining are 30 with low battery, then the racer could choose to drive conservatively and save energy. On the other hand, if our model would predict the number of remaining laps to be 30 with high battery power, then the racer could choose to drive aggressively and expend energy. Either way, if the racer can better manage their battery expenditure, then that would lead to a better strategy at winning the race. 

<br>

## Real Time Prediction
<br>
Since we are predicting the total number of laps with respect to each match, if implemented, our real-time predictions to the racer would be as follows : 
<br>
<br>

Image

<br>
<br>

## Data
<br>

The data that we used for this case competition has been provided by Genpact (https://www.genpact.com/). The data is arranged in a hierarchical format as follows :

```bash
├── data 
│   ├── Season 
│   │   ├── Location 
│   │   ├── ├── Friday Practice Stats
│   │   ├── ├── Qualifying Match Stats
│   │   ├── ├── Final Race Stats
```
<br>

Essentially, a few of the features included in the various datasets were as follows:
1) S1, S2 and S3 lap times<br>
2) Driver License number and Driver name<br>
3) Team Number<br>
4) Class<br>
5) Top Speed<br>
6) KPH<br>
7) Pit Time<br>
8) Total Time <br>
9) Total Laps Completed (upto that point in time)<br>
<br>

Few of the weather data features are as follows :<br>
1) Air temperature<br>
2) Track temperature<br>
3) Humidity<br>
4) Pressure<br>
5) Wind Speed<br>
<br>

## Feature Engineering
<br>
<br>
Because most of our data was in a hierarchical format of of files and folders, we took following feature engineering steps to clean and aggregate our data:<br>
1) 

 
