# CCU-Database
Technology to capture carbon dioxide (CO2) is already a reality and CO2 can be captured from various sources. 

The main questions though are the price of the capturing and what to do with the captured CO2.
 
For example capturing all the CO2 emissions that a coal plant is producing would consume almost a third of all the energy that the plant is producing.

In some cases captured carbon dioxide can be stored for example in emptied oil and gas wells. In this case we are talking about Carbon Capture and Storage (CCS).

Captured carbon dioxide can be also used for something that substitutes use of virgin raw materials. For example a Finnish energy company Fortum is capturing CO2 to create non-oil-based plastics for plastic industry use and technology company Solar Foods is making edible protein from the captured carbon. Both of these processes are called Carbon Capture and Utilization (CCU).

CO2 Value Europe is a non-profit association launched in 2017 representing the CCU value chain in Europe.

CO2 Value Europes is hosting and updating a comprehensive CCU database as one of its projects.

Link to the database: https://database.co2value.eu/

Database has great functionalities to sort and find data about completed, ongoing and upcoming CCU projects. Still, for a person interested in getting a big picture overview and running different analyses on CCU projects it would be great to have a database also as a CSV file. 

For this purpose the CO2 Value Europes database was scraped and downloaded as a CSV file. 

From this repository you can find the full CSV file under the name ‘co2_value_europe_database_cleaned.csv’ and 3 notebooks documenting the process of the database scraping. 

Data was scraped on October 11. 2023. Updates to the database after this day are not included to the CSV file. 

P.S To ensure that web scraping activities are legal and ethical, followed steps are recommended to take:

1. Check the Website's Terms of Service: Look for a "Terms of Service" or "Terms and Conditions" page on the website. Read through these terms to see if web scraping is explicitly prohibited or if there are any usage restrictions. Some websites may allow web scraping for personal use but prohibit automated or large-scale scraping.
   
In the CO2 Value Europes webpage there was no mention about prohibiting web scraping.

2. Check for a Robots.txt File: Many websites have a "robots.txt" file that specifies which parts of the site can or cannot be crawled by web crawlers or scrapers. You can check if the website has a robots.txt file by visiting the webpage and adding /robots.txt to the end of the website's URL. Review the rules in the robots.txt file to see if scraping is allowed or restricted for specific pages or directories.

URL_1: https://co2value.eu/robots.txt 
Respond_1:

Disallow: /wp-content/uploads/wpforms/ # START YOAST BLOCK # --------------------------- User-agent: * Disallow: Sitemap: https://co2value.eu/sitemap_index.xml # --------------------------- # END YOAST BLOCK 

URL_2: https://database.co2value.eu/robots.txt 
Respond_2:

*# See http://www.robotstxt.org/robotstxt.html for documentation on how to use the robots.txt file # # To ban all spiders from the entire site uncomment the next two lines: # User-agent: * # Disallow: /*

Results:

URL_1 respond Respond_1 prohibited access to this specific directory:  /wp-content/uploads/wpforms/ 

No other restrictions were found so web scraping to the database was done. 

