---
title: "Ethics and Legality of Web Scraping"
teaching: 45 # teaching time in minutes
exercises: 0 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- When is web scraping OK and when is it not?
- Is web scraping legal? Can I get into trouble?
- What are some ethical considerations to make?
- What can I do with the data that I’ve scraped?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After completing this episode, participants should be able to...

- Discuss the legal and ethical implications of web scraping
- Establish a code of conduct

::::::::::::::::::::::::::::::::::::::::::::::::

## The rights, wrongs, and legal barriers to scraping 

The internet isn’t as open as it once was.
What used to be a vast, freely accessible source of information has become a valuable reservoir of data —especially for training machine learning and generative AI models.
In response, many social media platforms and website owners have either started monetizing access to their data or taken steps to protect their resources from being overwhelmed by automated bots.

As a result, it’s increasingly common for websites to include explicit prohibitions against web scraping in their Terms of Service (TOS).
To avoid legal or ethical issues, it’s essential to check both the TOS and the site's `robots.txt` file before scraping.

You can usually find a site's `robots.txt` file by appending `/robots.txt` to the root of the domain—for example: `https://facebook.com/robots.txt` (not `https://facebook.com/user/robots.txt`).
Both the TOS and `robots.txt` will help you understand what is allowed and what isn’t, so it’s important to review them carefully before proceeding.


::::::::::::::::::::::::::::::::::::: challenge

Visit [Facebook's Terms of Service](https://www.facebook.com/terms.php) and its [robots.txt file](https://facebook.com/robots.txt). What do they say about web scraping or collecting data using automated means? Compare it to [Reddit's TOS](https://redditinc.com/policies/user-agreement) and [Reddit's robots.txt](https://www.reddit.com/robots.txt).

::::::::::::::::::::::::::::::::::::::::::::::::

In addition to reviewing a website’s policies, you should also be aware of the laws that apply in your region —especially those related to copyright and data privacy.
If you’re planning to collect a large amount of data for research or commercial purposes, it’s a good idea to seek legal advice before proceeding.
If you’re affiliated with a university, there’s a good chance it has a copyright office or legal team that can help you navigate the legal aspects of your project.
The university library is often a great starting point for finding support and guidance on copyright and data use.

To conclude, here is a brief code of conduct you should keep in mind when doing web scraping:


1. **Ask nicely whether you can access the data in another way**.
If your project relies on data from a particular organization, consider reaching out to them directly or checking whether they provide an API.
With a bit of luck they might offer the data you need in a structured format, saving you time and effort.

1.  **Don’t download content that’s clearly not public**.
For example, academic journal publishers often impose strict usage restrictions on their databases. 
Mass-downloading PDFs can violate these rules and may get you —or your university librarian— into trouble.

    If you need local copies for a legitimate reason (e.g., text mining), special agreements may be possible.
Your university library is a good place to start exploring those options.

1. **Check your local legislation**.
Many countries have laws protecting personal information, such as email addresses or phone numbers.
Even if this data is visible on a website, scraping it could be illegal depending on your jurisdiction (e.g., in Australia).

1. **Don’t share scraped content illegally**.
Scraping for personal use is often considered fair use, even when it involves copyrighted material. But sharing that data, especially if you don’t have the rights to distribute it, can be illegal.

1. **Share what you can**.
If the scraped data is public domain or you’ve been granted permission to share it, consider publishing it for others to reuse (e.g., on datahub.io).
Also, if you wrote a scraper to access it, sharing your code (e.g., on GitHub) can help others learn from and build on your work.

1. **Publish your own data in a reusable way**.
Make it easier for others by offering your data in open, software-agnostic formats like CSV, JSON, or XML. 
Include metadata that describes the content, origin, and intended use of the data.
Ensure it’s accessible and searchable by search engines.

1.  **Don’t break the Internet**.
Some websites can’t handle high volumes of requests.
If your scraper is recursive (i.e., it follows links), test it first on a small subset.

    Be respectful by setting delays between requests and limiting the rate of access.
You’ll learn more about how to do this in the next episode.

Following these guidelines helps ensure that your scraping is ethical, legal, and considerate of the broader web ecosystem.


## Other notes
- Boundaries for using/modifying user-agents
- Obey robots.txt
- Respect rate limits
- If unsure contact site administrator to seek permission to scrape
- Copyright laws - can legally scrape publically available data but republishing or reusing data may require permission

:::::::::::::::::::::::::::::::::: keypoints
- Always review and respect a website’s Terms of Service (TOS) before scraping its content.
::::::::::::::::::::::::::::::::::::::::::::
