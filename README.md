# Stock_Analysis

## Overview

&emsp; There are two important elements to stock anaysis: **Accuracy** and **Speed**. It is vitally important to accurately know a few vital factors about stock performance across a number of different stocks, but it is just as important to be able to get this information as quickly as possible across an incredibly large data set. In this analysis, we were tasked with optimizing both of these factors. First we needed to get Steve accurate information about a variety of tickers, and then we were tasked with optimizing the code in order to replicate this analysis more efficiently. While a few seconds or miliseconds does not necessarily make or break this analysis, optimizing the code and running time allows Steve to take this same script and expand it from 12 tickers, to 120 without breaking his computer. 


## Results

### Stock Performance

#### 2017
&emsp;2017 was decent year for these 12 stocks with all but one yeilding posititve returns. *DQ* and *SEDG* both almost hit a 200% return over the course of the year. *FLSR* doubled in value while maintainint significantly higher daily volume than any other stock. *DQ* had the lowest trading volume which could this stock to be a bit of a risk with lack of interest in the company. 

![2017](https://user-images.githubusercontent.com/109319148/183313884-909941ef-7172-47cd-9ad6-21b7c32d74ad.png)


#### 2018
&emsp; 2018 was not a great year for these stocks with only *ENPH* and *RUN* ending the year with positive returns. *ENPH* did quite well with the highest daily volume by far and a positive return of 82%. *RUN* also had a return in the high 80%s and the second highest trading volumes. 

![2018](https://user-images.githubusercontent.com/109319148/183313925-0fe1842a-b84a-4be1-a987-f362025bd0a2.png)


#### 2 year Analysis
&emsp; Looking across both years, *ENPH* would have been the best investment looking at the percentage return of 130% in 2017 and 82% in 2018. However, this was an extremely low share price on this stock, so doubling or tripling in dollar value isn't as exciting unless someone is buying a significant amount of shares. Usually a stock advisor, like Steve, would probably reccomend a portfolio of stocks balancing risk. One of the factors would a stock like *ENPH* that starts trading around $1 in 2017 and would be a bit risky although it had huge potential to grow with minimal investment for a meaningful amount of shares. 

&emsp; *SEDG* would also not have been a bad choice to hold for this two year period. While it fell 8% in 2018, the two year return was still well over 150% rising from a share price of around $13 to around $35. 

&emsp; While Steve's parents might not have made the most profitable investment if they had gone all in on *DQ*, they still would have been in the green with positive returns over the 2017 - 2018 time frame.
![2-year](https://user-images.githubusercontent.com/109319148/183314378-651cbc27-554f-4999-867e-0f50598554ea.png)


### Running Time
&emsp; Refactoring the code improved running time making it almost 10 times fasterer. In the image below, the top image represents the first attempt at the code, while the image on the bottom represents the refactored code. This means we could theoretically run 10 times as many stocks in the same amount of time.
![old_VS_new](https://user-images.githubusercontent.com/109319148/183314644-d7e0de4e-fbff-4b6e-9d39-0874790efd61.png)

2017 and 2018 both ran in minimal time as seen by these two images:
![VBA_Challenge_2017](https://user-images.githubusercontent.com/109319148/183314662-944897c5-79ce-4ffc-bbdc-4c6a7e249124.png)

![VBA_Challenge_2018](https://user-images.githubusercontent.com/109319148/183314679-a8a76079-f995-46c9-a797-c2d5ac45839c.png)

&emsp; Using an index for the stock tickers allowed us to create several more ouptut arrays and loop through the data quicker. This script also did not hold nested for loops that could be hogs on memory and processing time as in the first example. The file below shows 1 button for the original analysis and a second for the refactored challenge :
[VBA_Challenge.zip](https://github.com/ErinLVigil/Stock_Analysis/files/9277762/VBA_Challenge.zip)


## Summary

&emsp; There are clear advantages to refactoring this code namely in the ability to scale this project for the amount of data points or the amount of stocks. Right now we are only looking at a few key measures of performance for a stock, but refactoring the code allows us the ability to add in more factors without sacrificing processing time beyond our original model. There are other things such dividends, for example, that we could add into this analysis.  

&emsp; Disadvantages are a bit harder to come by. If this is a one time analysis, it might not be worth the time and effort to go back through a code that works quite well in order to optomize it. It might be a better use of time to map it out and write it in a suboptimal way than to spend the effort to work back through it. Loops also ensure that all data is run and displayed the same. I can imagine there might be a case where you might want to treat certain ticekrs differently, however it does seem like that would be a stretch. If you are not the primary owner of the code, refactoring someone else's code might be very challenging if you don't understand some of the nuances.

&emsp; Honestly, the original code for this worked fine and we do not really notice any difference in terms of running time. I am not able to accomplish more in my day with an extra milisecond or two. For Steve's purpose, our original code, while not overly pretty, worked just fine and was suitable for his needs of only a small subsector of the market. The extra couple of hours to refactor the code were useful for educational purposes and for a future project, but not needed to help Steve. Loops and arrays made it more difficult to understand the pattern of what was happening, and made it more likely an amateur, such as myself, was going to make a mistake. 
