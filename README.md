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

<p align="center">
<img src="https://user-images.githubusercontent.com/23395833/82750382-6d8c7700-9dcd-11ea-978d-59337cb29fd9.png" alt="Image"/> <img src="https://user-images.githubusercontent.com/23395833/82750384-6ebda400-9dcd-11ea-93a3-499d910a550e.png" alt="Image"/>
</p>


(left) - It shows BOX PLOT of each type of restaurant with it’s rating. Green
Triangle shows mean. We see mean values are comparable and similar to
each other. With extreme high and low values being seen in ‘delivery
types’.

(right) - It shows the frequency count of top cuisines with north Indian and
Chinese being highly preferred.

* Below we see word cloud for the positive and negative reviews.

<p align="center">
<img src="https://user-images.githubusercontent.com/23395833/82750452-e8559200-9dcd-11ea-9345-e542c60cbd2d.png" alt="Image"/> <img src="https://user-images.githubusercontent.com/23395833/82750470-091de780-9dce-11ea-9a11-851e3581d338.png" alt="Image"/>
</p>

High frequency words have a large font.

(left) - Word Cloud of Top 3 Restaurant reviews. We see ‘good’, ‘service’ tags showing positive sentiment.

(right) - Word Cloud of Least 3 Restaurant reviews. We see ‘WTF’, ‘bad’ tags showing negative sentiment.

* Below are the location density of restaurants according to various criteria on map.
  
  <p align="center">
  <img src="https://user-images.githubusercontent.com/23395833/82750795-3ec3d000-9dd0-11ea-80ac-23975e5622db.png" alt="Image"/>
  </p>
  
  This is the **location density of restaurants**. We can see that almost all restaurants are located near the centre of Bengaluru.
  
  <p align="center">
  <img src="https://user-images.githubusercontent.com/23395833/82750915-53ed2e80-9dd1-11ea-8673-b41e6ae821d3.png" alt="Image"/>
  </p>
  
  This is the **rating distribution of restaurants**. We can see that highly rated restaurants are clustered together.

  <p align="center">
  <img src="https://user-images.githubusercontent.com/23395833/82750946-8860ea80-9dd1-11ea-844c-49d42e836b85.png" alt="Image"/>
  </p>
  
  This is the **distribution of cost per person**. We can see that expensive restaurants are clustered together.

## Hypothesis Testing
### ‘Revenue’ increases when we switch from ‘offline orders’ to ‘online orders’?

We used the revenue predictive model to answer this.

We calculated difference between online order revenue and offline order revenue.

9265.04 - Difference between *Online* and *Non-online* revenue for originally *Non-online*.

This shows that revenue does increase when you switch to online orders.

-17362.65 - Difference between *Online* and *Non-online* revenue for originally *Online*.

This shows that revenue decreases when you switch to offline orders.

<p align="center">
<img src="https://user-images.githubusercontent.com/23395833/82751149-f35ef100-9dd2-11ea-8546-5fbeb4df0e00.png" alt="Image"/>
</p>

**Conclusion** - We **can’t be sure** whether the switch to take online orders will increase revenue or not. This is also confirmed by the above graph.

### ‘Revenue’ increases when we switch from ‘not booking’ to ‘booking’?

We used the revenue predictive model to answer this

We calculated difference between booking table revenue and not booking table revenue.

172646.94 - Difference between *Booking Table* and *Non-Booking Table* for originally *Non-Booking Table*.

This shows that revenue does increase when you start booking tables.

308789.35 - Difference between *Booking Table* and *Non-Booking Table* for originally *Booking Table*.
This shows that revenue does increase when you start booking tables.

<p align="center">
<img src="https://user-images.githubusercontent.com/23395833/82751311-e989bd80-9dd3-11ea-8b95-af5ff656dbf2.png" alt="Image"/>
</p>

**Conclusion**- Hence, we *can be* sure that switching to table booking increases revenue. This is confirmed by the above graph.

### Revenue is highly correlated with votes and cost per person. Also, cost per person should be highly correlated with *book table*.

<p align="center">
<img src="https://user-images.githubusercontent.com/23395833/82751397-7e8cb680-9dd4-11ea-94f8-ad756c3a22e5.png" alt="Image"/>
</p>

**Conclusion**- *Votes* is highly correlated with the *revenue* but the cost per person is only slightly correlated.
Also, *cost per person* shows a high correlation with the *book_table*.


### Highly rated restaurants have higher chance of offering online services and book table facilities.

<p align="center">
<img src="https://user-images.githubusercontent.com/23395833/82751453-02df3980-9dd5-11ea-9610-60c847cd647e.png" alt="Image"/> <img src="https://user-images.githubusercontent.com/23395833/82751454-04106680-9dd5-11ea-8581-31aca2f73d53.png" alt="Image"/>
</p>

We can see from the left plot that low rating, as well as high rating restaurants, have high chances of offering online order services.

We can see from the right plot that the *rating* increases as table booking services become more probable.

**Conclusion**- Offering Online order does not guarantee a high rating, but, offering table booking service does increase ratings.

## Predictive Modeling

### Restaurant Rating prediction
