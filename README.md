# pymaceuticals-assignment

In this assignment we were tasked with cleaning and analyzing data from cancer-drug trials on mice.

To clean the data we had to merge two CSV files, one containing mouse metadata and the other containing the drug regimen data. We merged this into a single dataframe on the "Mouse ID" column. There was also one mouse who had duplicate timepoint entries (and conflicting data from the trial), and this data had to be removed since there was no way of knowing which set of data was accurate.

Proceeding with data from 248 subjects, we calculated summary statistics (mean, median, variance, standard deviation, and SEM) using two methods: (1) calculating and compiling a dataframe separately, and  (2) using the .aggregate() function.

Our first visualization of this data included a bar graph of the total measurements taken for Tumor Volume in the different drug regimens. Two methods were used to plot these bar graphs: (1) DataFrame.plot and (2) pyplot.

Our second visualization of the data examined the sex of mice in the trials (which was found to have virtually a 50/50 split between female and male). The two methods for plotting were used in this case, as well.

To provide further analysis on 4 of the drug regimens (Capomulin, Ramicane, Infubinol, and Ceftamin), we iteratively calculated the quartiles, interquartile range, and upper/lower bounds for the final tumor volume and identified any potential outliers. This information was provided for each drug regimen in a printout. One potential outlier was found in the Infubinol regimen.

Our third visualization plotted these 4 drug regimen results in a box-and-whisker plot, visually representing the potential outlier from the Infubinol regimen.

For our fourth visualization, we sampled one mouse's data at random from the Capomulin regimen, and plotted it's tumor volume over time. This cell can be re-run over and over again, and each time it will generate a new mouse's data, selecting a sample at random.

Finally, our last visualization was a scatterplot that looked at the average tumor volume versus mouse weight. We ran a linear regression and found a relatively high correlation coefficient, plotting the linear regression model on the scatterplot and listing the equation.

A brief set of observations & discussion about the data analysis is provided at the end of the notebook.
