Data 301 Group 38A Final Report

**Our repository can be found here: <https://github.com/ubco-W2022T2-data301/project-group-group38> , along with relevant code and outputs for you to study!**

**Introduction**

Our project focused on the Airbnb listings for the state of Hawaii from this dataset <http://data.insideairbnb.com/united-states/hi/hawaii/2023-03-16/data/listings.csv.gz> . Both members of our group are new to data science and were unsure of what area we wanted to focus our project on. After looking through the datasets provided by Dr. Firas Moosvi in the canvas course shell, a group member expressed an interest in analyzing the listings of Airbnb rentals in Hawaii as he has spent time vacationing on the island and plans to continue visiting. After analyzing the dataset we quickly realized that there were many intriguing aspects and the group decided we would focus our attention on this dataset.

**Question 1:** **Which Island provides the most value based on price and quality of stay?**

To begin my analysis, I needed to find out what the different types of listings were on this dataset so that I could come up with average prices that reflected the type of room that was being listed. I quickly realized that while there are 4 room types in the dataset, two of them (Private rooms and Entire homes and apartments) make up most of the listings.

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/CPic1.png)

Once I realized this, it became clear that focusing my analysis on these two room types would be most efficient and provide enough information to answer my research question. I also concluded that any data regarding price or quality of stay should be split by these room types to get an accurate picture of the value of each listing type.

Here are the visualizations I created to demonstrate the average prices of both room types on each island:

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/CPic2png.png)

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/CPic3.png)

Once I had analyzed the price information, I needed a measure of the quality of stay and I discovered that the dataset included information about the reviews of each listing. I decided that using these review scores would be an effective way to uncover the value of each listing type and came up with average review scores.

Here are my figures outlining the average review scores for each island and room type:

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/CPic4.png)

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/CPic5.png)

Rather interestingly, the review score data was very similar and suggested to me that most visitors enjoyed their stay regardless of the room type or island, and that perhaps price is the most important factor.

Once this analysis was complete, I created the following report:

**Maui:**

**Private Room**

Average Price: **$606.71**

Average Review Score: **4.76/5**

**Entire home/apt:**

Average Price: **$753.44**

Average Review: **4.82/5**

### **Honolulu**
**Private Room**

Average Price: **$756.31**

Average Review Score: **4.71/5**

**Entire Home/Apt**

Average Price: **$346.82**

Average Review Score: **4.69/5**

### **Kauai**
**Private Room**

Average Price: **$485.07**

Average Review Score: **4.78/5**

**Entire Home/Apt**

Average Price: **$474.73**

Average Review Score: **4.75/5**

### **Hawaii**
**Private Room**

Average Price: **$508.79**

Average Review Score: **4.79/5**

**Entire Home/Apt**

Average Price: **$432.23**

Average Review Score: **4.77/5**

This report was used to answer my research question: **Which Island provides the most value based on price and quality of stay?**

**Answer:** Based on the findings provided above, there is answer for this question, but it is broken down by room type.

Private Room: Kauai 

Entire Home/Apt: Honolulu

**Question 2: What are the correlations between bedroom, price, and review score?**

I wanted to see what conclusions I could derive from review score, bedroom, and price data.

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/APic1.png)

Firstly, I made a heatmap of average review score per island. It is important to note that they are all very high scores, but the smallest of differences could be the most meaningful impacts for a traveller looking for the optimal experience.

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/APic2.png)

Then, I did average review score by room type using this scatter plot. Entire homes were much more commonly listed, as you can tell from analysis done in Question 1, which may have skewed the data for having higher average review scores.

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/APic3.png)

Between the islands, it seems as though Maui gets the most amount of high reviews. 

Now that we have an understanding between for review scores, I will move on to price and bedroom correlations.

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/APic4.png)

It can be drawn from this chart that there is a steady increase in price, as one would expect, from an increasing number of bedrooms. It is interesting to note that a 8 bedroom rental property is where one would get significantly more value than a 10 bedroom place. It is also interesting to note that there is a significant price hike when going up to 9 bedrooms from 8 bedrooms, in more than **double** the price.

For travellers in big groups, noting this difference could prove beneficial.

How many places are there by each bedroom count?

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/APic5.png)

As noted above, 8-bedroom listings are where travellers could get the most value. However, it is unfortunate that they are only available for basically half of the year, and there is so few of them. If travellers are looking to travel in big groups, they must be on the hunt for these few 8-bedroom deals that could be available!

However, they will have to settle with something less than a 5.0 review. As noted above, there are only 4 listings that have 5.0 reviews. Thus, it is not reasonable to expect to get the best of the best having 8 bedrooms.

![Alt text](https://github.com/ubco-W2022T2-data301/project-group-group38/blob/main/images/APic6.png)


**Findings**

**What is the average review score on each of the islands?** - I found that the average review score was very similar, all very high. This tells me: - Slight differences in review scores could reveal big differences for the ultimate travelling experience. Due to Hawaii's beautiful nature, reviewers may be skewed to leave better reviews anyhow. Small differences, and 5.0 rated houses, could make all the difference in terms of elevating one's travelling experience.

**Do the number of bedrooms have an influence on average review score, and how much does it affect price?** - It was found that number of bedrooms does not influence the review score, or price very much. Once again, travellers may be skewed towards giving higher reviews, because Hawaii is so beautiful.

**Are there any bargains for a certain number of bedrooms?** - It was found that 8 bedroom places offer significantly more value than any other bedroom size. Although far and few between, as visualized above, finding these places can provide great savings for travellers in large groups.

**Which islands have the best location scores?** - It was found that although only minor changes, "The Big Island" Hawaii, Hawaii had the best average review scores. For travellers looking for the ultimate location experience, The Big Island is where you want to go, offering the highest quality Airbnb's to stay at.

**Question 3: When traveling to Hawaii is it better value to stay at a hotel or book a private Airbnb?**

When deciding between staying at a hotel or booking a private Airbnb in Hawaii, there are several factors to consider. A traveller should consider the following information to make an informed decision based on preferences. To Begin  my analysis I had to compare the provided dataset with average hotel rates based on similar attributes to the listings.

**Cost:** Generally, Airbnb tends to be more cost-effective compared to hotels. However, it may depend on the location, season, and amenities offered.

<img width="982" alt="Screenshot 2023-04-18 at 11 48 16 PM" src="https://user-images.githubusercontent.com/122840406/233005495-daae149c-a221-415e-ac31-9c9c913a3a44.png">

Based on the above analysis I found that on average is it 10% less for a vacation rental compared to a hotel in Hawaii. 

**$227 is the average hotel room cost in Hawaii.**

After formulating the above bar graph I realized that hotel rates per night do not include resort fees or parking costs. These are minimal but could add up to over $50 per day. The cost varies depending on where you stay so I have furthered my research to provided a more accurate cost breakdown. I have broken down my data into subcategories; luxury, upper upscale class, upscale class, upper midscale class and midscale/economy class.

<img width="1581" alt="Screenshot 2023-04-19 at 1 07 44 AM" src="https://user-images.githubusercontent.com/122840406/233010609-8bcc0481-e9fa-47f3-b96f-249d5b761477.png">

**Bottom Line:** Plan to add $40 – $70 to the cost of your hotel room each night to cover resort fees and parking.

Adding an average of $55 extra per day in fees puts the average hotel cost at **$282.**

The Hawaii tourist board provides some information, but they don't do a very good job of tracking the prices of vacation rentals. Here is the data I could gather.

**$205 is the average daily rate of a vacation rental in Hawaii.**

<img width="1194" alt="Screenshot 2023-04-19 at 1 13 53 AM" src="https://user-images.githubusercontent.com/122840406/233012229-8236fa9a-d49d-4ba3-b20e-95222d49c5d3.png">

After factoring the added costs of staying a hotel the the average vacation rental in Hawaii is 28% less compared to a hotels. 

The primary source of cost savings when opting for a vacation rental in Hawaii is as follows:

* Exemption from resort fees (and possibly parking fees)
* The ability to cook meals at home and avoid expensive dining out
* Availability of vacation rentals with multiple bedrooms, which is more economical than booking multiple hotel rooms.

**Is opting for vacation rentals truly more cost-effective than staying at hotels in Hawaii?**

**Answer:** In summary, if you are a solo traveler or a couple who prefers dining out during vacation, selecting a mid-range vacation rental over a mid-range hotel may not result in significant cost savings. However, for families who plan to prepare some meals at the vacation rental, renting a vacation home can be a much more economical option, providing substantial savings.

Ultimately, it depends on your preferences and priorities. If you prefer a more home-like experience and privacy, an Airbnb might be the way to go. On the other hand, if you value the convenience of a hotel's amenities and services, a hotel might be a better option.

**Conclusion**

In conclusion, there were a lot of interesting data points drawn from this dataset that could provide of significant use for travellers. Which islands, how many bedrooms, quality of airbnbs, location/review scores, price, etc... all provide useful information for finding the best deals and best bargains for travelling to such a beautiful place. It was a lot of fun working with this dataset throughout the term!
