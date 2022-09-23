# Online Scraping Trial


I use Beautiful Soup to do this challenge. The website I choose is Reformation. I scrapped 30 items in this notebook. This logic is as follows: <br />
Step 0: create empty list for all the information we want <br />
Step 1: scrape the content on the clothing page. Count the number of items we have <br />
Step 2: Loop through each item. For each item, I scrapped its individual link, and then find its detailed description. In each loop, append each piece of information we want to the empty list that I created in step 0 <br />
Step 3: Using a pandas dataframe to store all lists. <br />


If we want to scrape all the items on the website, we can use nested loop. <br />
Step 0: scrape all element in the navigation bar on the top left cornor.<br />
Step 1: repeat all steps mentioned above in each navigation bar<br />



After we finish all scrapping, we use psycopg2 to establish the connection between python and postgreSQL. We transform pandas dataframe to sql dataframe, and upload/update all information we have. 
