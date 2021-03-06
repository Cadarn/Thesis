The data for the setting of sentiment aspect-based opinion mining is collected by scrapping methods from the Airbnb system. The text reviews that are scrapped are actually open to view for the public or Airbnb users. The data collection consists of two databases of two countries: Netherlands and United Kingdom. The dataset of the Netherlands consists of 34.028 listings. \\ Will this change?

The format of data for each of these listings is shown in the figure below. What I can get from the [JSON file](https://gist.github.com/AntigoniKourou/c28b087e0267f72f7163) is 
* The ID of the listing    **_id** or **review_vote:listing_id**
* The name and ID of the host    **reviewee:host_name** and **reviewee:id**
* The ID of the review    **review_id**
* Reviewer name and ID    **reviewer:host_name** and **reviewer:id**
* The text data    **comments**
* The number of reviews per listing **reviewData:metadata:reviews_count**

![](https://github.com/AntigoniKourou/Thesis/blob/master/logos/review_data_example.png)
![width=3cm]( https://github.com/AntigoniKourou/Thesis/blob/master/logos/actual_review.png)

These opinions have to be structured into structured data as below. 
(ej, ajk, soijkl, hi, tl),
* **ej** - a target entity: Named Entity Extraction (more)
* **ajk** - an aspect/feature of ej: Information Extraction
* **soijkl** - is sentiment: Sentiment Identification
* **hi** - is an opinion holder: Information/Data Extraction
* **tl** - is the time: Information/Data Extraction