# Data Science Project

## Aim
Analyse the Zomato Dataset to get an idea about the factors affecting the
establishment of various types of restaurants at different places in
**Bengaluru**, along with ratings, votes and reviews.

We also made predictive models about various parameters of a restaurant.

We also suggest a user how much revenue he/she can expect to earn by opening a restaurant with the provided restaurant parameters.

## Dataset
We used Zomato dataset available on [Kaggle](https://www.kaggle.com/himanshupoddar/zomato-bangalore-restaurants). We cleaned this dataset to obtain the final [dataset](https://drive.google.com/open?id=1oZR5CVixCDSUVG1rRex-DJxu34bqN7MM).

## EDA 
* 
| ![download (3)](https://user-images.githubusercontent.com/23395833/82749610-f2749200-9dc7-11ea-810f-10f128394a7c.png) | ![download (2)](https://user-images.githubusercontent.com/23395833/82749609-f1dbfb80-9dc7-11ea-86bb-db893d790517.png) |
|:---:|:---:|

These plots show the most expensive and cheapest places to dine.

*
![download (4)](https://user-images.githubusercontent.com/23395833/82749677-79296f00-9dc8-11ea-8654-3e6bcd561607.png)

North Indian Cuisine is most popular.

*
![download (5)](https://user-images.githubusercontent.com/23395833/82750382-6d8c7700-9dcd-11ea-978d-59337cb29fd9.png) ![download (6)](https://user-images.githubusercontent.com/23395833/82750384-6ebda400-9dcd-11ea-93a3-499d910a550e.png)

(left) - It shows BOX PLOT of each type of restaurant with it’s rating. Green
Triangle shows mean. We see mean values are comparable and similar to
each other. With extreme high and low values being seen in ‘delivery
types’.

(right) - It shows the frequency count of top cuisines with north Indian and
Chinese being highly preferred.

* Below we see word cloud for the positive and negative reviews.

![download (7)](https://user-images.githubusercontent.com/23395833/82750452-e8559200-9dcd-11ea-9345-e542c60cbd2d.png) ![download (8)](https://user-images.githubusercontent.com/23395833/82750470-091de780-9dce-11ea-9a11-851e3581d338.png)

High frequency words have a large font.

(left) - Word Cloud of Top 3 Restaurant reviews. We see ‘good’, ‘service’ tags showing positive sentiment.

(right) - Word Cloud of Least 3 Restaurant reviews. We see ‘WTF’, ‘bad’ tags showing negative sentiment.

* Below is the location density of restaurants according to various criteria on map.
  
  * ![image](https://user-images.githubusercontent.com/23395833/82750795-3ec3d000-9dd0-11ea-80ac-23975e5622db.png)

