# Notes on Crawling for very specific information.
Job postings, that is.

#### The first step is the URL frontier. 
The hope is to be able to find the URL with the relevant information. This part is kinda hard to do extremely well since the URL given the company might be completely different from the URL containing job postings, specifically ones that contain the actual clickable "Apply" button.

The goal of grabbing the relevant URL is to be able to give it to a webscraper. When you have the right URL, the webscraper can do it's job of gathering inforamtion. But! It needs the right URL. 

#### There's a big problem, though. 
Where are all the Jobs??? Unfortunately, they're everywhere. Or more accurately, anywhere. 

1. Posted on the company website.
2. Posted by a third-party website, like an ATS or literally any any site dealing with HR, payroll, or people. (Greenhouse is well-known, and Gusto is payroll but supports job postings???)
3. Linkedin Jobs
3. A founder or recruiter posting a position on linkedin. Apply in the coomments (wtf)
4. A developer repposting their boss's linkedin job post. 

It's this evolving process to find the best talent. This is all nice and dandy, but it's a pain in the ass to find these things anywhere they exist. Most of them are done like this due to a fundamental problem in hiring, which is this: how do we hire great people, and not hire not great people? The best way to hire is to not hire. What if instead of having embezzled resumes and job posts with unusual requirments, we could just find the best people and hire them? 

Best people == Best fit. 

There's too much missing information on both resumes and job postings, and this is unnecessary nowadays. 

## Level 1
The obvious way to crawl a site is to look for common paths like `/careers`, `/careers/`, or `/jobs`. Good job, you’ve done it! 

You can also try and guess full URLs for job postings. There are a ton of ATS sites that post jobs. Common ATS platforms include Ashby, Greenhouse, Workday, and Lever.  
 - Greenhouse: boards.greenhouse.io/<company> (has a public Job Board API).
 - Workday: <subdomain>.myworkdayjobs.com/<...> (e.g., company.wd5.myworkdayjobs.com)
 - Lever: jobs.lever.co/<company> (public endpoints for job boards documented in Lever Help Center)

## Level 2
You can parse the header or footer at the bottom of a website. You can crawl sitemaps. There’s also Job Posting Schemas. There's also APIs for job postings.
