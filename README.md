# Election_Analysis


## Project Overview
A Colorado Board of Education employee has asked for some help with auditing a recent local congressional election. They want to know about county-based results (which had the biggest turn-out, and what percent of the total vote each county accounted for) as well as candidate-based results (number of votes and percentage, as well as overall winner.)

## Resources
- Data Source: election_results/csv
- Software: Python 3.7.2, Visual Studio Code 1.58

## Election-Audit Results
- There were 369,711 total votes in the congressional election
- Jefferson county had 38,855 votes (10.5% of total votes)
- Denver had 306,055 votes (82.8%)
- Arapahoe had 24,801 votes (6.7%)
- Charles Casper Stockham had 85,213 votes (23.0% of total votes)
- Diana DeGette has 272,892 votes (73.8%)
- Raymond Anthony Doane had 11,606 votes (3.1%)
- The winner was Diana DeGette with 73.8% of the overall votes (272,892)

## Election-Audit Summary
By simply changing the file_to_load variable we could use the same script for any election. Granted, we would need to verify that the header columns are the same as the current data set. Additionally, we would need to verify that the data has been scrubbed and is not missing values. We could also modify this by combining the county-based results with the candidate-based results to get a breakdown of vote percentage per candidate by county. To accheive this we would need to create a new dictionary that has a key value of a combo of the county/candidate. We would initialize the dictionary to be empty and add in keys as we come across new ones, making sure to initialize to 0. Then we would increment the value for a key in the dictionary for all rows in the data. Lastly, we would use float division to calculate a percentage for all 9 candidate/county combinations. 
