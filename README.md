# Singapore_Bike_Visualization

### A 3D visualization of shared bikes in Singapore.
![General](https://github.com/ricardoCyy/imgs/blob/master/Sin_web/avg_trip_spatial.png)

**"What will a city look like if shared bikes are unleashed from docking stations?"**
The so-called dockless bike-sharing bussiness brings us the oppertunity to sketch the city in different spatio-temporal resolutions with largely collected and well organized precise GPS data. Visualization gives unambiguous and visible answers to that question we mentioned above under different scales/contexts.

### Spatio-Temporal Pattern:
#### 1. At *hourly* resolution
Hourly differences of arrival trips (Destinations) during a randomly picked **weekday** in each **250m** redius hexagon of Singapore. On morning peak ([7am-9am](https://en.wikipedia.org/wiki/Rush_hour#Singapore)) destinations are concentrated in HDB towns in singapore(home), while on evening peak ([6pm-8pm](https://en.wikipedia.org/wiki/Rush_hour#Singapore)) the destinations are diverse, which means ***shared bikes in Singapore are solving the first mile problem in morning.***[1]
![Hourly](https://github.com/ricardoCyy/imgs/blob/master/Sin_web/one_day.gif)

#### 2. At *weekday-weekend* resolution
On weekday, cycling activities are concentrated in particular areas of Singapore which show similar spatial pattern with **higher** amount([37%](https://youtu.be/_yfiuV4j9Jw?t=60)) on weekends, while slight differences are observed in outdoor attractions(e.g. [Marina Bay](https://www.google.com/maps/place/Marina+Bay+Sands,+Singapore/@1.3033138,103.8120058,11.75z/data=!4m5!3m4!1s0x31da19042950679d:0x7e9eb96cc0e8d6f2!8m2!3d1.2833754!4d103.8607264), [East Coast Park](https://www.google.com/maps/place/East+Coast+Beach/@1.3287831,103.8228122,11.88z/data=!4m12!1m6!3m5!1s0x31da22b906ff05d1:0xaffda4da354a96fa!2sEast+Coast+Park!8m2!3d1.3007842!4d103.9121866!3m4!1s0x31da187774c4d073:0x6dc2e74a10c148fc!8m2!3d1.2991943!4d103.9112697), etc.)
![WeekdayWeekend](https://github.com/ricardoCyy/imgs/blob/master/Sin_web/weekday-weekend.gif)

### Spatial:
#### 1. Near MRT
Shared bikes show strong connection to public transport, we use MRT as an example. Around [50%](https://youtu.be/_yfiuV4j9Jw?t=71) bike trips happen within 500m of MRT & LRT stations no matter it's on weekday or weekend.
![MRT](https://github.com/ricardoCyy/imgs/blob/master/Sin_web/near_station.gif)

#### 2. Community detection
Most trips are short in distance from which we can easily generating spatially cohesive communities using community detection algorithm([Blondel et al.](http://arxiv.org/abs/0803.0476)).
![CommunityDetection](https://github.com/ricardoCyy/imgs/blob/master/Sin_web/community_detection.gif)

### Weather:
#### 1. Rain or Not
Raining has notable effect([20% decrease generally](https://youtu.be/_yfiuV4j9Jw?t=80)) on bike demands.
![RainorNot](https://github.com/ricardoCyy/imgs/blob/master/Sin_web/rain_or_not.gif)

We have [an awesome video](https://www.youtube.com/watch?v=_yfiuV4j9Jw) about these contents above and further researches to support travel demand forecast and fleet size management will come soon.
The visualiztion and parts of analysis & data collection are done by me.
The codes will be shared in this repository soon.
