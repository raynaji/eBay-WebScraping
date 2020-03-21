# eBay-WebScraping

In this project, I web-scraped both sponsored and non-sponsored "playstation 4 slim" items on eBay website.

After obtaining the information of "seller name, seller score, item price, # items sold, best offer available, title, returns allowed, shipping price, condition", I created a local database to store all these information. 

With some further statistical analysis using SQL, I identified some features of differentiating sponsored and non-sponsored items.

Tasks to complete:
* Study the eBay URL to find out terms for search, page number, number of items per page, buy it now.  
* Identify and differentiate SPONSORED/NON-SPONSORED items. I introduced two ways to do it. One is by regex, another is through HTML class.  
* **Put item URLs into two text files:** Loop through 10 pages, separately identify sponsored and non-sponsored items. Put their URLs into different text files.  
* **Download item pages into two folders:** Open and read the two files containing item URLs. For each item URL, download the item page to the corresponding folder. Each item page should be named as "item_id.htm".  
* **Parse downloaded pages:** For each downloaded item page in the folders, parse them into Python project.  
* **Identify and store page elements:** Then identify the required HTML elements of the item page and store them. (seller name, seller score, item price, # items sold, best offer available, title, returns allowed, shipping price, condition). 
* **Insert values into SQL database:** Create database and table. Import the previously stored info into the table.  
* **Stats analysis:** Use SQL in Python to run summary stats analysis on each item.
