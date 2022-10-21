![image](https://user-images.githubusercontent.com/85826239/197128277-1650bf36-4c70-4ec2-9727-601ef3149cd3.png)

# San-Francisco-Airbnb
How can Airbnb outearn tranditional renting?

Set in San Francisco city, this project is targeted at real estate investors who might be wondering if listing their properties with Airbnb would earn more than renting to a long-term renter.

For this analysis, an Airbnb listing is deemed more lucrative if it earns more income per year than a 12-month rent.

The question is answered by analyzing the **`listings`** and **`calendar`** datasets made available by the courtesy of [Inside Airbnb](http://insideairbnb.com/get-the-data), along with the Zillow Observed Rent Index ([ZORI](https://www.zillow.com/research/data/)), a smoothed measure of the typical observed market rate rent across a given region.

The main success metric is **total revenue,** calculated by multiplying average daily rate by occupied rooms. *Note:* revenue does not consider expenses, so it can’t give a true picture of profitability and operating success.

Other variables needed for this analysis:
- **Popularity/Frequency of stays:** `number_of_reviews` are categorized into five bins:
  
    - 0-10 reviews: *New*
    - 11-25 reviews: *Rising* 
    - 26-50 reviews: *Trending*
    - 51-100 reviews: *Popular* 
    - 100+ reviews: *Hot*
- **Occupancy rate:** The percentage of occupied rooms, calculated by dividing the total number of rooms occupied, by the total number of `availability_365`, times 100.
