# Stock-analysis
#Challenge
Refactoring the code for the Green Stocks exercise to make it more efficient.  

In this analysis we were able to re-arrange the code so that the computer only had to read through the data file once, rather than for each value of the ticker variable.
This was done by creating array variables for volume, starting and ending prices.
A ticker index was created and set to zero outside the loop so that the value at the beginning of the loop is always zero.  For volume we then added (from 0 to 11, i.e. each ticker)
the volumes for each row to the value of the previous row.  
We then added one to the ticketindex at the end of the code inside the loop so that at the next pass the ticker value would be the next value in the tickers array.
We avoided having to use a nested loop which also saves resources.


