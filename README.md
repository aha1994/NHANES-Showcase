# NHANES-Showcase

A page to show some of the tools built as part of the Data Science Upskilling unit during my time with the CDC.

This tool was built using a python Flask app serving as the back end to download, process and return data to the React.js application on the front end. Data is retrieved from [here](https://wwwn.cdc.gov/nchs/nhanes/Default.aspx).

User's select a survey period and then choose from publically available variables. Afterwards they can choose a graph type to visualize the data. A few examples:

### Scatter Plot

A scatter plot of two biomarkers of smoke exposure

![Scatter Plot](https://github.com/aha1994/NHANES-Showcase/blob/main/Photos/Scatter.PNG)



### Multiple Box Plot

A box plot of a biomarker of smoke exposure by monthly family income brackets.

![Box Plot](https://github.com/aha1994/NHANES-Showcase/blob/main/Photos/Box%20plot.PNG)



The following features are currently being developed in a jupyter notebook before integrating them into the React.js application:


This tool allows users to select a variable, mean type, set of sample weights, and optional domain and max value limit to get weighted results in table form with 95% confidence intervals. When used correctly, these results reproduce values in the CDC's National Exposure report, found [here](https://www.cdc.gov/exposurereport/index.html).

### Exposure Report

Arithmetic Mean Serum Cotinine values with weighting.

![Exposure Report](https://github.com/aha1994/NHANES-Showcase/blob/main/Photos/national%20expoure%20report%20match.PNG) 


This tool below is used to visualize trends of different variable measurements weighted on population data. The user can download a graphics interchange format (gif) file that flips through variable histograms of each survey year. For each frame of the gif, identical x and y axis scales will be used so that it is easy to see how values change across different survey years. There are a few parameters the the user can use to modify the histogram output.

### Smoking Exposure over Time Gif

Histogram of weighted serum cotinine (biomarker of smoke exposure) values over time.

![Exposure Gif](https://github.com/aha1994/NHANES-Showcase/blob/main/Photos/LBXCOT_histogram.gif) 


This tool allows users to compare the distribution of laboratory results of the US population by Gender or Race. Comparative weighted histograms are displayed, showing an accurate representation of the percentage of each subpopulation in the US at each range of values. This tool is useful for identifying disparities in exposure and/or biological health measurements for different groups in the US. Users may select the year, variable, and domain (subgroups) they would like to see represented. The user can also edit the number of bins, log transform the x-axis and/or, limit the data to examine more detailed visual comparisons.

### Comparison of Blood Mercury Values by Race

Histograms of weighted blood mercury values by race

![Comparison](https://github.com/aha1994/NHANES-Showcase/blob/main/Photos/Blood%20mercury%20differences.PNG) 