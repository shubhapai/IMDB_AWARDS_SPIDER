IMDB Spider
===========

To run this code you need to have [Python 2.7](https://www.python.org/downloads/) installed on your computer and you need to have [Scrapy 0.24 installed](http://scrapy.org/)

## The Current State
Currently this spider starts at the imdb top 2014 year movie page. It then goes through each film copies its title, and the link url, then goes to each film page intern and collects a good chunk of the data avalible.It goes a page deeper using the links on the movie page and grabs awards detail as well. It then goes and sends that data to the Scrapy pipeline, where there is some cleaning that is done before it's finally saved into a sqlite3 db. 

