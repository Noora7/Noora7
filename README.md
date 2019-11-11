# 1.Introduction
To understand how and why attention, which is measured in terms of count of ratings, develops around the new products —— different kinds of  gift card, 4 plots are created by Python to visualize the attention raised during the first 6 months these new products first launched, as well as how it evolved. The timestamped data of the giftcards is collected from Amazon data  (2018 version) which contains reviews (rating, text, and helpfulness) and metadata(descriptions, category information, price, brand, and image features), and links(also viewed/also bought graphs).(J.McAuley, 2019). This study mainly focused on the rating of gift card, price, and product-market category data. The line chart is used to measure the relationship between the trajectory in the count of ratings and time. The distribution of rating times in different price levels and product-market categories is shown in the bar chart. The regression analysis indicates the factors which contribute to the development of consumers’ attention. 

# 2. Justification of the critical design decisions against the visualization wheel 
While making critical design decisions, visualization wheel proposed in Cairo's book is considered. Since the audience of  this chart is an experienced marketing analysts team, and the aim of the chart is to visualize the attention got by new products, the chart should be able to serve both exploration and presentation goals. As a result, balance should be sought between two flavors of professional backgrounds. 

To make the chart design decisions, six aspects are considered as following(Cairo, 2012):

- abstraction-figuration: A highly figurative chart uses physical representations to describe phenomena, while the emphasis shifts to abstraction when representations become conceptual. In our decision, charts are made in the form of one line chart, two bar charts and  a 3-D regression model, which is more close to abstraction but still clearly reveal the attention that the marketing analysts need.
- functionality-decoration: The four charts produced are not merely representation of data, colorful lines and bars, as well as 3-D model, are used to visualize the data. However, the charts are not heavily decorated, in order to reach a balance.
- density-lightness: While considering the density, the first three charts are more close to lightness, as only the relationship of two variables in each chart and comparatively small number of data is analyzed. And the fourth one is produced close to density, as association among three variables are discussed, a relatively large amount of data is used. As a whole, the style of charts are balanced but slightly close to lightness.
- multidimensionality-unidimensionality: Multidimensional graphics invite viewers to explore many aspects, while unidimensional graphics focus on one or few things. In these four charts, only on relationship in each is discussed. To make everything clear, the charts are designed to be more close to unidimensionality.
- originality-familiarity: Common and readable graphs such as line graphs are more close to familiarity, new forms of graphs are more close to originality. The first three charts, one line graph and two bar charts, are comparatively common and as readable as text, while the last one is quite new and challenging. After all, the design is balanced and slightly close to familiarity.
- novelty-redundancy: A chart that explains many things at one time can be viewed as novelty charts, while redundancy graphs are the opposite. In order to strike a balance between, the four charts explain one or two aspects at one time without using any data more than once. A balance is reached between novelty and redundancy.

# 3. Visualization and discussion of the association between the trajectory in the count of ratings and time, price, and market-product category 
## 3.1 The association between the trajectory in the count of ratings and time
![plot1]( 
Plot1 shows the count of ratings received in each of the first 6 months after the new products gift cards first launched. There are 9 categories in gift cards that had ratings during the time period, including all electronics, amazon home, cell phone & accessories, computers, health & personal care, software, toys & games, video games and general gift cards. 

One of the categories —— general gift cards received over 4000 ratings in the first month launched, which increased slightly in the second month but showed a decreasing trend during the following months, to approximately 1500 ratings in the sixth month. 
For the other 8 categories of gift cards, their counts of ratings fluctuated between 0 and 25 during the first 6 months after launching, and the numbers are quite small while compared to the category —— general gift cards.

## 3.2 The association between the trajectory in the count of ratings and price
In terms of the product attributes provided in the metadata, the product price and category are selected. The bar chart below identified the relationship between price and the count of ratings. Among the whole products in the gift card market, the gift card owns  the most wide range of price. First of all, while looking at the icon of product price and rating, it’s clear to see that gift cards includes the occasional price range from the 0 to NaN. In the total 1400 count of ratings, we focus on the 400 in order to have a clear view of the data distribution, products with 25-50 prices occupy nearly 150 points, and products with 50-75 scores occupy the second place, followed by products without pricing. The remaining products are basically evenly occupied The rest of the ratings. When we focus on other products, we will find that Amazon home scores only exist in three price ranges, namely 0 to 25, 25 to 50 and unpriced products. Similar distribution also exists in video games and toys & Games. Office products and undefined products (NaN) have a similar score distribution, which is reflected in 25-50, 75-100. The remaining product ratios do not show its price range, only show the number of scores he has obtained.

To conclude, a basic trend can be clearly seen from the main category gift card in the chart that: the higher the price, the more the count of rating is received in amazon.



## 3.3 The association between the trajectory in the count of ratings and product category
Another product attribute is the product category. The whole gift cards market is segmented into different parts including 13 types of gift cards listed in the x axis, such as Amazon Home, Health & Personal Care, Gift Cards and etc.. The bar chart indicates that the count of rating for Gift Cards is larger than 1400, which is the largest among those products. To better visual  and compare the distribution of all kinds of gift cards , the y-axis value was limited to the highest level of 100. 

The Gift Cards receive the most attention from buyers, therefore the product development apartment is expected to launch more new and popular products of the specific category named Gift Cards. Besides, consumers who bought Gift Card, Amazon Home, Toys and Games pay much more attention to the Gift Card (in purple color) in the Gift Card, Amazon Home, Toys and Games. On the contrary, the consumers of Health & Personal Care and Office products are more interested in the Gift Card Accessories (in red color) instead of Gift Card. These consumers prefer to send gift cards more formally. Therefore, the market analysts should concentrate more on the Gift Card Accessories in those two targeted product markets. For other 8 categories of gift cards, consumers only focus on the Gift Cards, which means the development of the Gift Card Accessories for those categories is expected to be paid less attention to.




## 3.4 The association between the pace, average rating and trajectory in the count of ratings  

The multiple regression model is built to explore whether the pace with which the ratings are posted, average rating affect the count of rating significantly. The time period is the first six months since the new gift cards were launched. The average rating of each day is the amount of sum Overall value listed in the Metadata dataset divided by days. Another independent variable is the ratio of the increase of rating times each month. 
In the statistical regression results showed in the table, the R square value and adjusted R square value are 0.101 and 0.100 separately. Both graphs indicate that there is no significant relationship between these two independent variables and count of rating. Thus, the pace with which ratings are posted and average rating do not account for the attention of consumers purchasing gift cards in the first month since they occurred in the markets.  
# 4. Conclusion
Overall, the graphs show that the price of the product account for the development of consumers’ attention towards gift cards, the higher the price, the more the count of rating is received. While considering the other attributes: firstly, time is examined, the count of ratings decreased since the second month (only considering the first six months after the product launched). Secondly, relationship with product category is discussed. There are two ways to categorize:1) 13 types, 2) with accessories or not. On one hand, the Gift Cards receive the most attention from buyers, on the other hand, consumers who bought Gift Card, Amazon Home, Toys and Games pay much more attention to the Gift Card itself in the Gift Card, Amazon Home, Toys and Games, while the consumers of Health & Personal Care and Office products are more interested in the Gift Card Accessories. However, while looking at the relationship among attention, pace and average rating by conducting a multi regression, little correlation is detected.
# 5. Limitation
Firstly, the short time span of data selected could make the results unreliable to provide  complete insights to explore the factors that account for the consumers’ attention. The data is only selected from 201 to , the first six-month since the new gift cards were launched. More data through wider time periods are expected to use in future studies. Secondly, the incompletely information could cause a bias in the statistical analysis. The dataset of Amazon gift card lacks price information especially for the gift cards which were rating more than about 340 times in the first six months. The lack of price information of those frequently rating products may lead to an unreasonable prediction about the relationship between rating and price of some popular products. Thirdly, Price is not selected from the raw dataset to be the independent variable in the regression as there is no timestamp data in the Meta dataset. The price value could not correspond to each count of rating accurately.  Further studies towards the relationship between price and the count of ratings in gift cards should be conducted. 


# References
Cairo, A. (2012). The functional art. p.62.
Jianmo Ni, Jiacheng Li, Julian McAuley(2019). Empirical Methods in Natural Language Processing (EMNLP) 




























## Group member
He Renjie, 
Huang Yilie, 
Meng Kejun, 
Yang Huize,
Zhou Nan
