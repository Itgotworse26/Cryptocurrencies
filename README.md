# Cryptocurrencies
Practice and Challenge Assignment for Module 18

# Background
You and Martha have done your research. You understand what unsupervised learning is used for, how to process data, how to cluster, how to reduce your dimensions, and how to reduce the principal components using PCA. It’s time to put all these skills to use by creating an analysis for your clients who are preparing to get into the cryptocurrency market.

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of your most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

# Screenshots
This was the crypto_df before pre-processing:

![crypto_df before pre-processing](https://github.com/Itgotworse26/Cryptocurrencies/tree/main/Resources/crypto_df_Before-Processing.JPG)


After several rounds of pre-processing; keeping all currencies being traded, assessing which currencies had a working algorithm, dropping any columns that had null value, keeping only currencies that have coins mined, and dropping the "IsTrading" and "CoinName" columns, this is what the crypto_df now looks like:

![crypto_df after pre-processing](https://github.com/Itgotworse26/Cryptocurrencies/tree/main/Resources/crypto_df_After-Processing.JPG)


After using PCA to reduce dimension to three principal components, we can create a pcs dataframe that uses the names of the cryptocurrencies as its index.

![pcs dataframe](https://github.com/Itgotworse26/Cryptocurrencies/tree/main/Resources/pcs_df.JPG)


Thanks to this, we are able to concat the crypto_df and pcs_df to create a clustered dataframe. 

![clustered dataframe](https://github.com/Itgotworse26/Cryptocurrencies/tree/main/Resources/clustered_df.JPG)


The clustered dataframe is then used to create this 3-D scatter plot:

![3-D scatter plot](https://github.com/Itgotworse26/Cryptocurrencies/tree/main/Resources/3-D_Scatter_Chart.JPG)


The clustered dataframe is also scaled using a MinMaxScaler and then used to create a plot dataframe, which is then used to create this scatter plot:

![scatter plot](https://github.com/Itgotworse26/Cryptocurrencies/tree/main/Resources/Scatter_Plot.JPG)

