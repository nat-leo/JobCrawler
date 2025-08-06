# JobCrawler
Job Hunt Like a Pro

## Definition of Done.
1. Webcrawler can take a company site and discover the job postings site or url.
2. Webcrawler is tested on accuracy using a list of "company: job site" a base accuracy is found.

## TODO
1. Create a set of 25 company sites and their job sites.
2. Design the webcrawler to scrape the site for associated URLS
3. Given associated URLs, webcrawler must scrape urls to identify whether or not the URL is Job Listings

#### Create a set of 25 company sites and their job sites. You're at 10/25 now
 - Put these in a tests folder.

#### Design the webcrawler to scrape the site for associated URLS
 - Use OpenAI as an Web Search Agent. Design a prompt to identify URLS from the base URL.
 - Measure accuracy by whether or not the crawl successful listed out the URL from the test companies. List this accuracy.

#### Given associated URLs, webcrawler must scrape urls to identify whether or not the URL is Job Listings

 - Use OpenAI as a Webscraping Agent. Design a prompt to search the URLs for Job Listings.
 - Measure accuracy by whether or not the crawl successful identified the right URL. List this accuracy.s

