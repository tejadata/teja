Data Transformations

 

In the real time most of the  variables are not normally distributed and most of the parametric  statistics test(ANOVA,T test, Regression etc..) are based on the  assumption that the data is normally distributed therefore it do not  meet the assumptions of statistical tests if the data is not normally  distributed,in this case the results will mislead the outcome.

 

The process of making data to near normal distribution is called normalization

 

Quick point why we should go for data normalization.

 

    To achieve linearity between variables

    To reduce the skewness of the data  (Not all normalization process will reduce the skewness of the data for  example Z transformation will not change any skewness of data where log  transform will do that) 

Logarithm:

Logarithm is one of the data  normalization method which is widely used mainly  to reduce the skewness  of the data. Logarithm are prone to negative and zero values.

If you see the below images from left  to right, left histogram is without log transformation were right  histogram is log transformation, you can see there is lot of difference  in terms of data distribution, and also if you observe the right  histogram we almost achieved normal distribution.

Click here to know how logarithm works.

 

 

                     Source medcalc

Scaling :

Scaling  is the  process to standardize the range of independent variables of data,  because each feature are in different scale and if you want to make it  in certain range (typically between 0 to 1).

 

Why do we need scaling?

 

        You can view sample dataset for x1 and x2 here, if  you see the data for x1 data range is high where x2 range is less  mostly in between 0 to 8, and mean difference between this two variables  also very high.In this case we will go for data scaling to reduce the  range typically between 0 to 1.

 

Below is the scatterplot between x1 and x2 before data transformation.

 

 

Now lets scale the data and plot the graph again.If you  observe the below scatterplot, only difference we can see is the scaling  of the values in X and Y axis and rest are same.you can view the data  from here after normalization(Used Z transformation).

 

 

How did I do the above scaling? They are many ways to do data scaling below are widely used one.

    Z score

    MinMax 

Z score: We already discussed this in few of our articles under distributions category, so let’s go straight into the formula for conversion/Normalization  

 

 

 

 

 

 

MinMax:This is one of the easy way to data normalization because it needs less computation power

 

 

 

 

 

 

Now let’s use the above three options to convert our data in to normalization, we will take first four observations from our dataset that is available for download here .

Mean for our dataset for x1 = 4674.04 and standard deviation = 3427.734

 

 

 

 

 

 

 

 

 

Z transformation:

 

 

 

 

Now once we applied Z transformation  for the four observation below is the result.

 

 

 

 

 

 

 

 

 

MinMax transformation:

In our dataset minimum values is 2028 and maximum value is 15427.

 

 

 

 

 

 

Now once we applied MinMax transformation  for the four observation below is the result.

 

 

 

 

 

 

 

 

Normalization and scaling will be obviously applied only on numeric values
