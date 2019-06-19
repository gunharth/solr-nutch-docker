
## How to use
```bash
docker-compose up
```

## How it works
A default Solr instance with the default "mycore" core is used to store Nutch crawling results.
The approach of this PoC is to use as less custom configuration as possible so it can be used as a starting point for other uses.
Some important files:
* seed.txt: The starting urls on which the crawl should start
* regex-urlfilter.txt: The filter which is used to only filter out targeted urls
* index-writers.xml: The Nutch config which is used to link Nutch and Solr
* docker-compose.yml: The infrastructure configuration, including the Nutch start command

## Adjusting this demo
* The ```/nutch``` folder contains all Nutch configuration

# Heavily based on the works of
* [Sebastiaan Raven](mailto:basraven@gmail.com)
