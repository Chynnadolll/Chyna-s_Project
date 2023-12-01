# Chyna-s_Project
first I Imported all the necessary library 
Pandas, numpy, matplotlib, seaborn, datetime, yfinance
then Initializing the dt
Start = “2006-01-01”
End = “2023-11-20
Then downloading all of stocks using yahoo finance with their tickers(indivually)
I then Set tickers for each bank 
Tickers =  signature bank, silicon valley bank, amazon, bank of america, Goldman sachs, morgan stanley, citigroup, jpmorgan chase
Now Using pd.concat to concentrate all of the banks together in a single dataframe 
Using stocks_df
Checked the first five rows using .head()
What can you say about Signature Bank?
The stock heighted around 2022 when the market was open
Immediately crashed in 2023 due to its closure on March 23, 2023 by federal regulators
Plotted using ticker[open].plot() and sns.despine
removes the spines from the right and upper portion of the plot by default
Repeated the same steps as before
Downloaded dated from jan 1st, 2006 to november 25th, 2023 using yf.download from yahoo finance 
Set all the tickers for the stocks
Using stocks.head() to check first five rows 
Downloaded all of the stocks within one dataframe
Set columns names to stocks
Adding bank ticker and stock info 
stocks.column.names= [‘Bank Ticker’,’Stock Info’]
Then checked the first 5 rows to see if it worked 
Asked to explore data more 
checked close prices for each stock 
Amazon: 187.57, bank of america: 54.90, citigroup: 546.01, Goldman sahcs: 423.85, jpmorgan chase: 171.78, morgan stanley: 108.73
Create a new dataframe called returns, contains each stock
Checked the head 
Which bank stock had the best and worst single day returns ?
Jpmorgan chase 
Min 01-20-2009
Max 01-21-2009
Cause of the worst drop in 3 banks?
President obama was sworn into office 
01-20-2009 = BAC, GS, JPM
Visualization of the data
Imported the needed library 
Matplotlib inline
Set the grid style to white grid 
Graph each stock using ticker[close].plot() and sns.despine()
Any relationship between this plot and the worst drop of these stock
For the worst drop date all the stocks significantly lowered below 100 (as seen in the last graph with all of the stocks plotted together)
Create a pairplot of the returns frame 
sns.pairplot(returns)
What stocks stand out to you 
In the bottom row I noticed that in all the stocks compared to MS they never really  went over 0.2 and i thought that was interesting 
Create a histogram plot for each of the stocks 
ticker[close].plot(kind=’hist’)
Compare all the stocks using a histogram
Used stocks[close].plot(kind=’hist’)
BAC had the most frequency  
calculate the moving average
Set start and end 
Download jpm and ms 
Set tickers 
Create the moving average by using windows for python and average 
JPM[Close'].rolling (window=30).mean0.iloc|0:599].plot (label=30 Day Avg)
JPM[Close').iloc|0:599].plotlabel='JPM Close)
