# Cryptocurrencies

### Project Overview

In this unsupervised Machine learning is used for processing the cryptocurrency market data. Since, its classified as unsupervised, there is no defined output, but we try to create report to include the traded cryptocurrencies group as per the features.In the process we are trying to help Accountability Accounting, a prominent investment bank, to build a new cryptocurrency investment portfolio for its customers.For the purpose, clustering algorithms and data visualizations are used.
Following are the expected deliverables:

   1. Preprocessing the Data for PCA
   2. Reducing Data Dimensions Using PCA
   3. Clustering Cryptocurrencies Using K-means
   4. Visualizing Cryptocurrencies Results

### Resources

Data Source: [crypto_data.csv](https://github.com/CorinneBean/Cryptocurrencies/blob/58315dc54d519f4fb36690b9b4b1129dd81b4fd1/Resources/crypto_data.csv) 

Software: Python , Anaconda Navigator, Conda, Jupyter Notebook , numpy, sklearn, pandas, plotly & hvplot
    
### Results 

The imported dataframe had 1252 rows X 6 columns. After data cleaning (including - only which are being traded , with not null Algorithm , Not null in other fields , and rows where coins are mined (TotalCoinsMined > 0)  and dropping few columns, we have a total of 532 tradable cryptocurrencies. 
After, getting the cleaned dataframe , the text columns are converted into numeric data using get_dummies() and also large value data columns are scaled using StandardScaler() , to avoid skewed data.After we implement PCA to reduce the dimension to three principal components.

### Clustering Cryptocurrencies Using K-means
An elbow curve is formed the K-Means method iterating on k values from 1 to 10. We consider 4 clusters , since there is a sharp changed at k=4. 

![Elbow Curve](https://github.com/CorinneBean/Cryptocurrencies/blob/58315dc54d519f4fb36690b9b4b1129dd81b4fd1/Images/Elbow%20Curve..png)

### Visualizing Cryptocurrencies Results

![3d scatter code](https://github.com/CorinneBean/Cryptocurrencies/blob/58315dc54d519f4fb36690b9b4b1129dd81b4fd1/Images/3d%20scatter%20code.png)

![3d scatter](https://github.com/CorinneBean/Cryptocurrencies/blob/58315dc54d519f4fb36690b9b4b1129dd81b4fd1/Images/3D%20Scatter.png)

A 3D-Scatter was created with the PCA data and the clusters. 


A 2D-plot showing the clusters , Create a hvplot.scatter plot using x="TotalCoinsMined" and y="TotalCoinSupply".Showing the 532 tradable cryptocurrencies, based on their Class for the 4 K_mean clusters obtained above. 

![scatter](https://github.com/CorinneBean/Cryptocurrencies/blob/58315dc54d519f4fb36690b9b4b1129dd81b4fd1/Images/Scatter.png)



The following image shows the 532 tradable cryptocurrencies in the form of a table using hvplot.table.

![tradeables](https://github.com/CorinneBean/Cryptocurrencies/blob/58315dc54d519f4fb36690b9b4b1129dd81b4fd1/Images/tradables.png)

 
