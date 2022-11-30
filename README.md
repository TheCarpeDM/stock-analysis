# stock-analysis

## Overview of Project
 
### Purpose
This analysis is for Steve who is looking for financial advice on what stocks to invest in. We looked at the performance of the stocks over the course of 2018 to determine their overall performance for the year. We wrote a VBA script so that he wouldn't have to install developer tools or even do more than press a button so that he could use this tool in the future.

## Results

### Stock Analysis
Steve's initial idea of investing in DQ might be a bad idea based on the 2018 data. DQ had the greatest decrease at -62.6% over the course of the year. ENPH and RUN were the only stocks we looked at that had positive performance over the course of 2018, so as long as that performance is expected to continue, those look like the best investments based on the data. Since the data being analyzed was the same between the initial script and the refactored code, they do not have any bearing on this portion of the analysis.

### Refactoring vs Initial Code
There was a marked improvement in processing time between the two scripts. Our initial script took 1.164 seconds to run:
 ![First Script Elapsed Time](/resources/VBA_Challenge_2018_First_Script.png)

 and the refactored script took only 0.164 seconds to run:
![Refactored Script Elapsed Time](/resources/VBA_Challenge_2018_Refactored_Script.png)

The 1 second difference in performance of the code between the Initial and Refactored scripts increases in importance the more often the code is used. If it saves Steve 10 seconds over the course of his day, the refactoring hasn't been very useful. If the code is used 300 times a day by a company of 30 stock traders, that has saved the company 2.5 hours worth of work, and suddenly that second is incredibly useful.

 
## Summary

Refactoring the code cut the processing time immensely. However, because of my misunderstanding of the instructions, finding what went wrong took FAR longer than the single second of difference was worth. In a larger data-set, or a script that would be used over and over again by numerous people every day, that increased efficiency might be worth the work, but in this case, a 1 second difference whenever Steve feels like checking his stocks is not worth the 2 hours I spent (not to mention the frustration) trying to figure out exactly what was causing my code not to work. The issue ended up being that I read the instructions as "create a for loop" in both parts 2a and 2b, but only 1 loop was actually needed.