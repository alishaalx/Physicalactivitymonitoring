# Physicalactivitymonitoring
This Jupyter notebook consists of the analysis,hypothesis testing and model building for the set of 9 subjects which includes an adult group of 8 males and 1 female and their corresponding readings taken by wearing three different Inertial Measurements Units and Heart Rate monitor.All the 9 adults were subjected to 18 different physical activities and the readings realated to their hand,chest and ankle were noted down.the information of each adult is then stored in a ".dat" files.
The process of this data analysis involves an approach is datacleaning followed by hypothesistesting which is then followed by model building.

Initial steps of importing all the required libraries and loading data from the list of files.

Data Cleaning:

Function : data_cleaning()
           Sub-Function :fill_null_heartrate() :- replace Null values of heart rate column

Exploratory Data Analysis:

Train,Test data splitting
Function : train_test_splitting() :- Splitting into train and test set

Correlation through heatmap
Function : genrate_heatmap() :- Generate Heat-Map

Time and activity Analysis with respect to the actvities undertaken by each subject
Function : elapsedtime_heartrate() :- Estimating Elapsed Time and mean heart rate for each subject and
            their corresponding activities

           Sub-Function : change_milllisec() :- convert calculated elapsedtime to seconds

Function : plot_scatter() :- Plotting a scatter plot between mean heart rate and elapsedtime(sec)

Activity Heartrate Analysis
Function: activity_heartrate() :- Analyse the heart rate for each activity for a subject at time


Hypothesis Testing:

Hypothesis stated : A hypothesis of dependency between activity and human heartrate fluctiations.
Function : con_cat() :- perform concatenation as per the requirement hypothesis testing
Perform z-test
Result based on z-test()

Modelling :

Prediction of heart rate done using polynomial regression and random forest
an example is illlustrated for both and predictions are obtained
