# Welcome to a hands-on exercise using **AI insights** in Power BI Dataflows to predict car price


## Setup Power BI Dataflow

1. Go to https://powerbi.com and Sign in
2. Create a workspace

![createbpiws](https://raw.githubusercontent.com/Azure/carprice/master/images/createbpiws.png)

3.	Give the Workspace a name like CarpriceDemo.  Note that the Workspace name must be globally unique so add you initials or pick something unique that works for you.

![pbiwsname](https://raw.githubusercontent.com/Azure/carprice/master/images/pbiwsname.png)

4.	Create new content
5.	Click on Get started under Dataflows

![dataflow](https://raw.githubusercontent.com/Azure/carprice/master/images/dataflow.png)

6.	Click on Add new entities

![newentity](https://raw.githubusercontent.com/Azure/carprice/master/images/newentity.png)

7.	Select Text/CSV as a Data source

![datasource](https://raw.githubusercontent.com/Azure/carprice/master/images/datasource.png)

8.	Paste the URL ``https://automlsamplenotebookdata.blob.core.windows.net/automl-sample-notebook-data/carprice.csv`` for the csv file carprice.csv
9.	Click `Next`

![csv](https://raw.githubusercontent.com/Azure/carprice/master/images/csv.png)

10.	Enter a Name for the query (like carprice)
11.	Click Save & close

![queryname](https://raw.githubusercontent.com/Azure/carprice/master/images/queryname.png)

12.	Name the dataflow (like carpriceDF)
13.	Click Save

![dfname](https://raw.githubusercontent.com/Azure/carprice/master/images/dfname.png)

14.	Click on Refresh now

![refresh](https://raw.githubusercontent.com/Azure/carprice/master/images/refresh.png)

15.	Click on the left most Edit entity icon in Actions

![editentity](https://raw.githubusercontent.com/Azure/carprice/master/images/editentity.png)

16.	Find the bore column.
17.	Click on the dropdown
18.	Click on Text filters

![editbore](https://raw.githubusercontent.com/Azure/carprice/master/images/editbore.png)

19.	Choose does not equal
20.	Enter ?
21.	Click OK

![doesnotequal](https://raw.githubusercontent.com/Azure/carprice/master/images/doesnotequal.png)

22.	Find the ``bore`` column again

![boreagain](https://raw.githubusercontent.com/Azure/carprice/master/images/boreagain.png)

23.	Click on the datatype ``ABC`` and select ``1.2 Decimal number``

![boredatatype](https://raw.githubusercontent.com/Azure/carprice/master/images/boredatatype.png)

24.	Find the ``stroke`` column
25.	Click on the datatype ``ABC`` and select ``1.2 Decimal number``

![stroke](https://raw.githubusercontent.com/Azure/carprice/master/images/stroke.png)

26.	Find the ``horsepower`` column
27.	Click on the datatype ``ABC`` and select ``123 Whole number``

![horsepower](https://raw.githubusercontent.com/Azure/carprice/master/images/horsepower.png)

28.	Find the ``peak-rpm`` column
29.	Click on the datatype ``ABC`` and select ``123 Whole number``

![peak-rpm](https://raw.githubusercontent.com/Azure/carprice/master/images/peak-rpm.png)

30.	Click Save & close

![saveclose](https://raw.githubusercontent.com/Azure/carprice/master/images/saveclose.png)

31.	Click on Refresh now

![refresh](https://raw.githubusercontent.com/Azure/carprice/master/images/refresh.png)

32.	Click on the left most Edit entity icon in Actions

![editentity](https://raw.githubusercontent.com/Azure/carprice/master/images/editentity.png)

33.	Click on AI insights

![aiinsights](https://raw.githubusercontent.com/Azure/carprice/master/images/aiinsights.png)

34.	Select the carprice model and click ``Apply``

![apply](https://raw.githubusercontent.com/Azure/carprice/master/images/apply.png)

35.	If you get this message click ``Continue``

![continue](https://raw.githubusercontent.com/Azure/carprice/master/images/continue.png)

36.	Review the carprice prediction in the Power BI Dataflow

![review](https://raw.githubusercontent.com/Azure/carprice/master/images/review.png)

37.	Click on ``Cancel`` so the next you use the Dataflow it is starting at the same point.  If you forgot you can just delete the last 3 steps up to and including “Invoked AzureML.carpricedemo” 

![invoke](https://raw.githubusercontent.com/Azure/carprice/master/images/invoke.png)
