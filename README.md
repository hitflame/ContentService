# ContentService
A video crawler,keeping track of the most recent videos from Internet

  This project started from one of my work about 2 years ago,it is used as a tool to crawl newest videos information to  provide content service for web pages.

  The whole system running on django framework,written in Python.All crawlers are written before,and when the system runs,it would create  multi-process to instance the crawlers in `ContentService/contentservice/crawlerimpl/`, then execute the crawling task.

  There are 2 kinds of  crawlers:ListCrawler and ContentCrawler,the former is used to crawl the video list  and saving the task into mongoDB
while ignoring the details about the video,the ContentCrawler executes the detailed task  fetched from mongoDB created by ListCrawler.
  
if you have any doubts while using this crawling tools,I'm glad to offer you some help O(∩_∩)O~
