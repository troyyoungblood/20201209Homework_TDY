# 20201209Homework_TDY
Homework Set 5
# Matplotlib Homework - The Power of Plots

Final notebook and images are contained in folder labeled Pymaceuticals_TDY

I. DATA CLEANUP

Before beginning the analysis activities were conducted, a check was conducted to determine if a mouse had duplicate data.  A mouse, ID g989 was identified as having duplicate data for several Timepoints.  The duplicate data was reviewed and determined that the values were close enough together to average the values versus throw the data away.  The respective duplicate row data was averaged, the duplicate rows were removed and the averaged data was inserted into its associated Timepoint row.

There were also 3 mice identified witinh the Ceftamine regimen as having started the study and did not finish.  All only had data at Timepoint 0.  A quick comprison using the summary statistics table was used to determine if there was an appreciable difference between those values when using all the mice for the Ceftamine regimen and a the full list minus the 3 noted above.  There was no real difference between the 2 summary tables and therefore, the 3 mice were left in the data to get results similar to others in the class.

II. DATA ANALYSIS

1) A Summary Statistics Table was created consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

2) The instructions state "Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin". 
 
 As written, the instructions are confusing.  Calculate means to do something.  It does not mean just grab a static data point. To generate useful data, I calculated the difference between the initial and final tumor volume.  This value is useful because it can be used to generate a rate and, more importantly, allows for the clear presentation of the effectiveness of the 4 drugs identified when plotted in a box chart. 
 
 The quartiles and IQR and were also quantitatively determined.  An outlier was identified for the Infubinol regimen, mouse id c326..
  
 III. DATA VISUALIZATION
 
 1) Bar charts were created showing the number of measurements taken per drug regimen. Image names are pandasbar_measvsregimen.png, pyplotbar_measvsregimen.png
 
 2) Pie charts were created to show the percentage of overall female and male mice. Image names are pandaspie_fvmdist.png , pyplotpie_fvmdist.png
 
 3) A box chart was created to clearly show which drugs were most effective at tumor reduction. boxplot_deltastatistics4reg.png
 The boxt chart plotted Difference in  Tumor Volume (Start - Finish) vs Drug Regimen.
 
 4) A line chart showing the reduction in tumor size over time for a select mouse on the Capomulin tv_time_Capomuline.png
 regimen.
 
 5) Scatter plot showing average tumor volume versus mouse weight.  scatter_avgtv_vs_weight_Capomuline.png
 
 6) A scatter plot with a linear regression line showing average tumor volume versus mouse weight.  regression_avg_vs_weight.png
