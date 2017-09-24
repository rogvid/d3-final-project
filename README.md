# Copenhagen Appartment Prices

## Design Decisions
This is the final project in my Udacity Nanodegree D3 course. I have chosen to visualize the data using a choropleth with colors representing price intervals. The map tiles I chose were low key to keep a low data-ink ratio, and the chosen color scheme was Plasma. The visualization uses martini glass storytelling, and has hover functionality so that postal district sales and average sales prices can be seen.

## Data
The data was scraped from Boliga.dk in early 2016, and has not been updated since then. The map for 2016, will therefore not be representative for the entire year of 2016. Futhermore I suspect that Boliga.dk doesn't have all data for all sales in the 1992-2016 period, since it is clear from the visualization that the number of sales per year is very small to begin with, and quite high at the end.

## Data Story
This visualization nicely captures the appartment price growth in copenhagen in the period 1992-2016. It is even possible to see a stagnation in the price development, most likely caused by the housing collapse in 2006 and the following economic crisis, and a subsequent resurgence in price growth.

## Price Growth Driving Factor and Possible Crash
One of the biggest driving factors behind the exponential increase in appartment prices is that you aren't taxed on the profit of a sale. Combine this with regulations in 1989, that increased what is known as "realkredit lån" - realkredit lån is essentially a very low interest loan on appartments - from 60% to 80% of the appartments sales price, as well as the city of copenhagen selling of many of their rental appartments, and what you have is a generation of people buying appartments for a fraction of their market value. These people, because of the zero taxation on profit, have since the early 2000's been able to either buy expensive appartments for their children, through what is called "forældrekøb", which is essentially parent purchase, by taking a loan in their own appartment, or they can invest in some of the expensive new appartments, which coincidentally are popping up everywhere in copenhagen, by simply selling their appartment, often with a 600+% ROI. Given that I see the price development as being way to steep, I do believe that we will see a big correction in the average sales price within the next 5 years.

## Feedback
As a part of the project, we had to ask people to review our visualization and give some feedback. I chose to post a question asking for feedback on the Data Analyst Nanodegree forum on Google+. Below I've listed the feedback, as well as the feedback I received from handing this project in the first time. Those who can see posts on this forum, can go [here](https://plus.google.com/u/0/104542938068928012184/posts/bLtqnMq42bi?cfem=1) to see the post.

### Feedback from Jagdeep Sandhu:
Liked your project. Good work.

### Feedback from Vagner Sanches Vasconcelos:
Very good.
I will adapt my data view to look similar to yours.

### Feedback from Hatem Kotb
Good stuff man! Btw, could you please double-check the data for Karlslunde? The average is quite high, a Danish friend of mine spotted it right away! :D I believe the 2010 data is specifically high relative to the others.

Again, good stuff! ;-)

### Follow-up: 
I looked into the question to double check the values for Karlslunde and responded with the following posts:

***Reply before looking into the data:***
>+Hatem Kotb Thank you. I'll have a look at the data, but as I wrote below the viz I don't think the site I scraped had information on all sales. Furthermore, because some years, had very few sales, a single large sale is sometimes shifting the average up by a large margin. I'll get back to you when I've looked at the data again 😊

***Reply after looking into the data:***
>+Hatem Kotb Hi again :) I would like to thank you for pointing this out. I have looked at it, and it does look very strange. If you look at the boliga site here http://www.boliga.dk/salg/resultater?so=1&sort=omregnings_dato-d&maxsaledate=2011&iPostnr=2690&gade=&type=Ejerlejlighed&minsaledate=2010&p=1, you'll be able to see all the sales in Karlslunde in 2010-2011. There are a bunch of appartments, all located at Egedal, which were all sold for 39.5 mil. kr. I have no idea what this is about and am looking into this now. But from another source I found that in 2006 one of the appartments there was sold for 50 mil. kr, so there is something strange about this place. But as far as the aggregated value in the visualization, it is correct, but the underlying data might be corrupted or incorrect. Thanks again :) 

### Feedback from Udacity Reviewer:
Formatting is consistent and effective, excellent work here. We recommend including use strict directive right under the opening \<script\> tag to set javascript into strict mode. This is useful to help you write a secure javascript. More information here. That being said, you have done a good job to meet this specification.

### Follow-up
Added the "use strict"; to the start of the script in the index file.