<h1> ETL Foundations Project </h1>

<img src="https://www.brandsvectorlogo.com/content/uploads/images/indeed.jpg" alt="Indeed.com">

## EXTRACT - Data Sources:
* Indeed.com - Web scrape Indeed.com Austin Jobs postings
* Census Data - API calls for Austin zip codes https://pypi.org/project/CensusData/

## TRANSFORM:
* Cleaning/filtering out unnecessary data
* Creating new columns for data comparison
* Loaded results to a dataframe.
* Zip codes needed to be casted into the correct data type (i.e. from float to integer)
* Zip codes needed to be extracted from address field (e.g. Austin, TX 78701)

## LOAD:
Mongo DB with three collections:
* First data source - Indeed job listings
* Second data source - Census data indexed by zip code
* Combined data

## Challenges:
* Pop-ups on Indeed.com result pages required a custom function to close them.
* Zip codes with leading zero's would have required padding with Python's zfill() method

## Lessons learned:
* Every web scrape project has site-specific problems requiring site-specific programming logic.
* API's are much easier to extract data from.

### Team Members:
* Jadd Cheng [@jlcatx512](https://github.com/jlcatx512/)
* Dundar Karabay [@dundarkarabay](https://github.com/dundarkarabay)
* Janie Lua
* Thuria Abdelaziz [@tkabdelaziz](https://github.com/tkabdelaziz/)