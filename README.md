# wattch-shop-analitics

This project I have analyzed data from http://watchshop.kz/ and https://time4u.kz. There were 
problems with the first site that it was not possible to inspect the site to view the tags, which 
created a lot of problems. As a result, there was a second site where the data met the conditions.
Let's move on to the scraping itself, that is, everything is very simple, using python tools, that 
is, beautifulSoup you can get data from the site itself.

First of all, I studied the site, it is simple and intuitive, there is a main page, and a page with 
a set of clocks. I chose a men's watch. Data on men's watches is only 60 pages, each page contains 
12 products, in total 720 pieces. The page stores data such as price and brand name, and detailed 
information is stored in a separate page dedicated to a specific product.

The detailed page contains information such as Brand, Warranty, Bracelet type, Glass, Case 
material, Water resistance, Calendar, Alarm, Time display. I assumed that the number of such fields 
should be enough, and proceeded to scrape. First of all, I created a project in Jupiter, loaded all 
the necessary libraries. And from the main page I collected all the links to the detailed page for 
each product. After, from each detailed page, I also collected all the characteristics. I wrote the 
received data to a file in csv format, so that every time I do not scrap the site, as it takes some 
time. At this point, the data collection phase is over.

### 
[Results](https://github.com/Moali123-svg/wattch-shop-analytics/blob/main/project%20Results.pdf)
