# Election-Analysis

### Overview
The goal of this project was to determine the results of an election, both the winning candidate and the county that produced the most votes. The raw data came from the polls in a CSV file. My task, then, was to count the votes and compile a report with the necessary information. 

### Methodology
The first decision to make was which tool to use. The file provide was an Excel CSV file, so VBA would have been a good choice. Were I the individual responsible for presenting the results, I may have elected to use VBA for its practical interface with Excel and ability to quickly produce graphs. In this case, though, my manager, Tom, only required a written report in a text file that he could easily access from Command Prompt. Thus, I decided that Python would be the tool to use for its ease of loading, creating, and writing to files. Python was also useful for its ability to use formatted print lines, which proved very practical in this project.

### Results
Here is a screenshot of the text file that will be sent to my manager, Tom.

![Election Results](https://github.com/veachk90/Election-Analysis/blob/main/Election_Results.png)

In this case, voter turnout refers to the number of voters from a given county, not the percentage of eligible voters who decided to actually cast a vote. From the data, we do not know the total of how many eligible voters existed in each county. If I had had access to this data, it would have been great to include in the final report. This would provide valuable information for future political candidates, as they could direct their efforts toward counties where voters vote and avoid those that do not, or possibly to find ways to inspire historically inactive voters to participate in the democratic process.

From the total number of votes this election, it was fairly straightfoward to calculate each of the relevant percentages for both counties and candidates. The winning candidate, of course, is the only one that can have more than 50% of the toal vote. Here is the result displayed in the command line, to ensure that it works when called from there as well:

![Election Results from the Command Line](https://github.com/veachk90/Election-Analysis/blob/main/Election_Results_Command_Line.png)

### In the Future
Because this script makes use of general variables and loops to add elements to list and dictionaries, it can be used to produce the same type of results in future elections, provided that the data is provided in the same format. One change that will need to be made for future use of this script is to update the names of the files to load and the files to save. In order to maintain an organized archive, we would want these names to reflect the date and location of each election. Another change to make would be to write a case in the unlikely event that there is a tie between two candidates. This script has no report to produce in such a situation, which would need to be added for the script to be considered for repeated implementation. 
