# scraping-google-maps-reviews
This repository shows how to scrape Google Maps' places reviews data using SerpApi. Total 3 places' reviews are scraped in this code file, by filtering only Indonesian reviews. Google Maps API has also been used to find out place_id for 3 places.
<h1>Motivation to do this project</h1>
I've been applying to AI/ML related tasks/jobs on <a href= "https://www.upwork.com/" target="_blank">Upwork</a>, and got this scraping job (which paid me 20$ to complete the scraping task). I had done some scraping before, but I got to learn a lot while doing this task. I tried using Selenium to scrape the data, but Google services are very restricted to scrape. Also, I tried Google Maps API but it has a limitation of only 5 reviews to scrape.<br> At last, I tried <a href= "https://serpapi.com/" target="_blank">SerpApi</a> from which I was able to scrape the google maps reviews data successfully. Although SerpApi is a paid service, we can use their Free Tier service in which they provide 100 requests limit per month.<br>
<h1>What is scraping</h1>

![image](https://github.com/sachelsout/scraping-google-maps-reviews/assets/86348193/f9973fef-6801-42cf-b052-285189541ac9) <br>
Python web scraping is an automated method used for collecting large amounts of data from websites and storing it in a structured form. If we try to do it manually, it requires a lot of time and manpower, also resulting in human errors. So it's always better to scrape the required data using Scraping. <br>
<h1>Step-by-step methods followed in this project</h1>
<ol>
  <li>Required installs/imports for serpapi, pagination, creating dataframes.</li>
  <li>Setting parameters for serpapi API calls for scraping maps data as well as places' reviews data.</li>
  <li>Make API call and get the required data in dict format. Do this for all the reviews using pagination.</li>
  <li>Extract reviewers' names and their reviews, store it in dataframe, filter only Indonesian reviews (API call scrapes both Indonesian and English reviews, sorting Indonesian reviews first. So locate where Indonesian reviews end and consider only those reviews).</li>
  <li>Create a CSV file to store these Indonesian Google Maps reviews.</li>
 </ol><br>
 <b>Note :- Follow the same above steps for remaining 2 google maps places.</b><br>
 <h3>Sample Indonesian reviews scraped - </h3>
 
 ![image](https://github.com/sachelsout/scraping-google-maps-reviews/assets/86348193/37ad86a1-b804-4e61-adc4-877823bcb12c)
