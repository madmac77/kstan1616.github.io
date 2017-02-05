![PairPlot](/images/Unknown-16.png)

In this project we were given a data set on several thousand loans and asked to build an algorithm that would predict whether
the loan would default or not. It was the first project that we have gone from start to finish alone and we were given relative free reign on how to structure our EDA and model- that's what made this project satisfying to complete. 



To begin I pulled in the data from the csv file we were given. With the data imported, I began by printing out the dataframe and 
selecting the columns of the dataframe that I would need for visualizing and modeling the data. With the data I needed, I began 
the process of cleaning the data. In particular, I removed some strings from a column and converted classification values into 
numerical types. With the data ready to be manipulated and graphed, I began to look at data in pivot tables and a few scatterplots.
Along with those graphs, Kilian showed me scatterplots which were great for seeing the relationships between a lot of variables
at once, and I repeated this experiment various times to see if I could spot another trend in the data. 

With graphs in hand, I moved onto normalizing the data. This wasn't too difficult as I had some borrowed code from a previous 
lesson and used a function to apply it to various columns of data. I began using ridge regression and actually came up with some decent values for my hyperparameters before realizing that we needed to use a Bayesian method. With that in mind I began building the model which at this point is becoming a little more intuitive.

With the values for my parameters I continued on to predict the outcome of several lines of data, of which I had the information of the loan status, and thus could verify if the model worked well or not. I found that my model does give higher probability to customers paying when they do (true positives) than customers defaulting, but the probability estimate is greater than 50% (the amount of defaults in the dataset) so there would be many false positives. 

I think I could better my model by simplifying it and building up from there, one by one, assuming that it was correctly done this time. Overall, I learned a lot in this project about RLS (although that wasn't the point of the exercise), cleaning data, using pandas dataframes, and improving my grasp on the statistical methods that we have been using. 

