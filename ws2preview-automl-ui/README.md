# Welcome to a hands-on exercise using the **Azure Machine Learning service** to author a model using the NEW **Workspace2 AML Preview Automated machine learning UI**


## Create an AutoML Experiment

1. Open the Azure Machine Learning workspace by clicking on it in the Azure portal

![openworkspace](https://raw.githubusercontent.com/Azure/carprice/master/images/openworkspace.png)

2.	Click on the **Launch Preview Now** button

``Contents of this page will be moving to a new immersive experience for managing the end-to-end machine learning lifecycle. Compute targets will be manageable from both locations. Features provided in preview are offered at no additional charge but may not remain so after general availability.``

Note you can also navigate directly to the new immersive experience [here](https://ml.azure.com/)

![portal](https://raw.githubusercontent.com/Azure/carprice/master/images/portal.png)

3.  If asked select your Subscription and Machine Learning Workspace.  If not asked move to Step 4.

![choosesubws](https://raw.githubusercontent.com/Azure/carprice/master/images/choosesubws.png)

Then click Get Started

![choosesubws2](https://raw.githubusercontent.com/Azure/carprice/master/images/choosesubws2.png)

4.  On the Home page click on the Create New dropdown and select ``Automated ML Experiment``

![automlexp](https://raw.githubusercontent.com/Azure/carprice/master/images/automlexp.png)

5.	Enter an Experiment name and click on Create a new compute

![expname2](https://raw.githubusercontent.com/Azure/carprice/master/images/expname2.png)

6.	Enter a Compute name, Select virtual machine size, set Minimum number of nodes to 0, set Maximum number of nodes to 6, and click Create

![createcompute2](https://raw.githubusercontent.com/Azure/carprice/master/images/createcompute2.png)

This may take a couple minutes

![createnewcompute2](https://raw.githubusercontent.com/Azure/carprice/master/images/createnewcompute2.png)

7.	Select a training compute and chose the new compute created above.  Click ``Next``

![amlnext2](https://raw.githubusercontent.com/Azure/carprice/master/images/amlnext2.png)

8.	Click on Upload from local file to upload the carprice.csv you downloaded in the prerequisites. Or get it from the path where you cloned this GitHub repo.  Give it a Name and click Next

![uploaddatasetbasicinfo](https://raw.githubusercontent.com/Azure/carprice/master/images/uploaddatasetbasicinfo.png)

9.  Review the setting and preview and click Next

![uploaddatasetpreview](https://raw.githubusercontent.com/Azure/carprice/master/images/uploaddatasetpreview.png)

10. Review the Schema.  Remove the ``symboling`` and ``normalized-losses`` columns

![uploaddatasetschema1](https://raw.githubusercontent.com/Azure/carprice/master/images/uploaddatasetschema1.png)

11. Change the Type of the ``price`` column to Integer.  Click Done

![uploaddatasetschema2](https://raw.githubusercontent.com/Azure/carprice/master/images/uploaddatasetschema2.png)

12.	Preview the data.

![previewdata2](https://raw.githubusercontent.com/Azure/carprice/master/images/previewdata2.png)

13.	We excluded a couple of columns earlier but if forgot Ignore the SYMBOLING and NORMALIZED-LOSSES columns (features) by clicking on the Included/Ignored slider

14.	Chose ``Regression`` for the prediction task and ``price`` for Target column. Click ``Start``

![regression](https://raw.githubusercontent.com/Azure/carprice/master/images/regression.png)

15.	Let it run to finish to complete the experiment.  Do this the first time ahead of the demo to have a completed experiment.

## Review the AutoML Experiment

Once the AutoML experiment completes 

1.	Click on the Run ID of the completed experiment

![runid2](https://raw.githubusercontent.com/Azure/carprice/master/images/runid2.png)

2.	View the Iteration Chart and view some of the point on the graph

![ichart2](https://raw.githubusercontent.com/Azure/carprice/master/images/ichart2.png)

3.	Scroll down to the Iterations and talk about the models and their Spearman Correlation

![spearman2](https://raw.githubusercontent.com/Azure/carprice/master/images/spearman2.png)

4.	Click on VotingEnsemble and look at the graph Predicted vs. True

![predvtrue2](https://raw.githubusercontent.com/Azure/carprice/master/images/predvtrue2.png)

## Deploy AutoML Experiment carprice model

1.	Click on ``Deploy Model VotingEnsemble``

![voting2](https://raw.githubusercontent.com/Azure/carprice/master/images/voting2.png)

2. Deploy Model, enter a Deployment name and click the Deploy button.

``Note that if you click the Deploy button it is going to take 5 to 10 minutes to deploy the model.  You will also have to delete the endpoint, so you are not charged on Azure to continue to run the compute in an Azure Container Instance (ACI)``

![deploymodel2](https://raw.githubusercontent.com/Azure/carprice/master/images/deploymodel2.png)

3. To see how the deployment is proceeding click on Endpoints in the Assets section of the AML service workspace2 to see the Endpoint.

![deployendpoint](https://raw.githubusercontent.com/Azure/carprice/master/images/deployendpoint.png)

4. To see how the deployment is proceeding click on the endpoint.  The State will be Transitioning until the endpoint is created and the State will change to Healthy  

![deploymentstate](https://raw.githubusercontent.com/Azure/carprice/master/images/deploymentstate.png)

5. After you are finished with the endpoint you can delete the ACI endpoint by clicking in front of the endpoint and clicking on Delete.  ``Note that you will only want to do this after the Power BI part is completed``

![deletedeployment2](https://raw.githubusercontent.com/Azure/carprice/master/images/deletedeployment2.png)

6.	Consume the ACI web service in Power BI by clicking [here](https://github.com/Azure/carprice/tree/master/powerbi)
