# BKK Basic Crawler

A tool that makes http requests and outputs the url and the content (optionally to file)

## How to run..

###  the tests

`go test`

###  the compiler 

`go build`

###  the program 

To fetch just one url

`./bkkCrawler http://www.mysite.com`

fecthing several urls (by default in parallel with 10 threads)

`./bkkCrawler http://www.mysite1.com http://www.mysite2.com`

specifying the number n = 2 of parallel threads (goroutines)

`./bkkCrawler -parallel=2 http://www.mysite1.com http://www.mysite2.com`

taking the urls from a file (text file with one ulr per line), in linux:

`xargs ./bkkCrawler -parallel=100 < urlslist.txt`

