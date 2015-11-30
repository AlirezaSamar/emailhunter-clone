EmailHunter Clone
=================

A simple python script that crwal Google for certain keywords, crawls the webpages and return all emails found.

Requirements
------------

- sqlalchemy
- urllib2

If you don't have, do `sudo pip install sqlalchemy`. 


Usage
-----

Start a query with a proper keyword, let's say "vox.com" as an example.

	python email_crawler.py "vox.com"

This process might take a while since it retrieve up to 500 Google search results and crawl up to 2 levels deep, something around 10,000 webpages!

Once the process finished, run this command to get the list of crawled emails

	python email_crawler.py --emails

The list of emails will be saved in ./data/emails.csv