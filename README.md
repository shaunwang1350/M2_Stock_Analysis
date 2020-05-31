# Challenge: M2_Stock_Analysis

In this Challenge, we are asked to refactor existing code that is provided to us. 

Press 'Analysis' button to begin Subroutine, and 'Reset' button to clear everything.

I began by chunking many of the existing formatting code (such as creating the worksheet Title, Ticker, Total Daily Volume, and Return) and placing it at the end of the subroutine. Then I proceeded to declare 4 arrays (Tickers, Volume, StartPrice, EndPrice). I elminated the for loop for setting volume as 0, since it can be completed within one for loop later. I also declared tickerIndex variable as 0 and RowCount as the bottom row of the dataset. Within the major for loop, I had four If statements that allowed me to:

1. Incrememt the ticker if the dataset's ticker does not match our existing ticker, and set volume array at tickerIndex as 0 (this eliminates having another for loop)
2. Add to the volume array at tickerIndex position if we are on the correct ticker. 
3. Set the startPrice if the previous cell is not our ticker and our current cell is our ticker.
4. Set the endPrice if the next cell is not our ticker and our current cell is our ticker. Within this If statement, I also included printing out the ticker, volume, return at tickerIndex to the All Stocks Analysis sheet and placed another If/Else statement inorder to give Returns red or green. (This eliminates having another for loop) A

Lastly, I have chunked the formating at the end so that it is cleaner code.
