# Welcome to a hands-on exercise using the **Azure Machine Learning service** to author a model using the **Notebook VMs**


## Create an Notebook VM

1. Open the Azure Machine Learning workspace by clicking on it in the Azure portal

![openworkspace](https://raw.githubusercontent.com/Azure/carprice/master/images/openworkspace.png)

2. Click on the Machine Learning service workspace.  You should now see a choice of ``Notebook VMs`` under Authoring.

![amlServiceWorkspaceOverview](https://raw.githubusercontent.com/Azure/carprice/master/images/amlServiceWorkspaceOverview.png)

3. Click on +New

![amlNotebookVMsConsole](https://raw.githubusercontent.com/Azure/carprice/master/images/amlNotebookVMsConsole.png)

4. Enter an Name for the Notebook VM, choose a VM size, and click Create

![amlNotebookVMsCreate](https://raw.githubusercontent.com/Azure/carprice/master/images/amlNotebookVMsCreate.png)

5. Notice how the status is `Creating`.  This is where you can go to Stop, Start, Restart, Delete, or Create Notebook VMs

![amlNotebookVMsConsole2](https://raw.githubusercontent.com/Azure/carprice/master/images/amlNotebookVMsConsole2.png)

6. After a few minutes the Status will change to `Running`.  Now you can click on the URI link `Jupyter`

![amlNotebookVMsConsole3](https://raw.githubusercontent.com/Azure/carprice/master/images/amlNotebookVMsConsole3.png)

7. This will open the Jupyter Notebook VM.  Navigate to your user folder.  My user folder for example is `darsch`

8. To open up a Terminal click on `New` > `Terminal`

![newTerminal](https://raw.githubusercontent.com/Azure/carprice/master/images/newTerminal.png)

9. type `ls` to list your user directory

10. type `cd userName` to change to your user directory (mine was `cd darsch`)

11. type `ls` to list the contents of your user directory

12. type or copy and paste ``git clone https://github.com/Azure/carprice.git`` to clone the GitHub repository

![terminal](https://raw.githubusercontent.com/Azure/carprice/master/images/terminal.png)

As above you can Clone this GitHub repository using the following commands: 

    `git clone https://github.com/Azure/carprice.git`

You might want to make a new directory prior to cloning (like creating a `repos` directory using `mkdir repos`)

13. Go back to you Jupyter Notebook Files and navigate to the `carprice` directory

![carpriceDir](https://raw.githubusercontent.com/Azure/carprice/master/images/carpriceDir.png)

14. Navigate to the `notebooks` directory

![notebooksDir](https://raw.githubusercontent.com/Azure/carprice/master/images/notebooksDir.png)

## Running the carprice regression.ipynb notebook in the Azure Machine Learning service Notebook VM

1. Open the `carprice regression.ipynb` file and select the Python 3.6 - AzureML kernel and click Set Kernel

![carpricereg](https://raw.githubusercontent.com/Azure/carprice/master/images/carpricereg.png)

2. Run the first cell in the Setup section of the notebook by clicking on the cell and Ctrl+Enter on keyboard 

![cell1setup](https://raw.githubusercontent.com/Azure/carprice/master/images/cell1setup.png)

3. Run the second cell in the Setup section of the notebook by clicking on the cell and Ctrl+Enter on keyboard 

![cell2auth](https://raw.githubusercontent.com/Azure/carprice/master/images/cell2auth.png)

4. Run the `Create or Attach existing AmlCompute` cell.  This cell is going to take about 5 minutes to complete.

![cell3](https://raw.githubusercontent.com/Azure/carprice/master/images/cell3.png)

5. Run the cells in the Data section

6. Run the cells in the Train section.  The remote_run experiment cell is going to run for a while (20 minutes).  Check it out in the Automated machine learning UI in the Authoring section of the AML service workspace 

![train](https://raw.githubusercontent.com/Azure/carprice/master/images/train.png)

7. Run the cells in the Results section

8. Run the cells in the Retrieve the Best Model section

9. Run the cells in the Register the Fitted Model for Deployment section

10. Run the Create Scoring Script cell

11. Run the Create a YAML File for the Environment cells

12. Run the Create a Container Image cell

13. Run the Deploy the Image as a Web Service on Azure Container Instance cells

14. Consume the ACI web service in Power BI by clicking [here](https://github.com/Azure/carprice/tree/master/powerbi)

15. If you uncomment the Delete a Web Service cell `#aci_service.delete()` you can delete the ACI webservice.  You can also delete from the Deployment Assets in the AML service workspace.

16. Run the Test section cells to test the web service in the notebook

17. Remember to delete the ACI deployment so you are not charged for the compute.  Unless you want to show it to the Power BI users in your organization.  Then use your learnings to deploy a model in your organization.

## Stop the Notebook VM

When you are done using the Notebook VM go back to the Notebook VMs console and click `Stop`.  You can return here to start it again, but this way you are not charged for compute while it is not being used.

![amlNotebookVMsConsole3Stop](https://raw.githubusercontent.com/Azure/carprice/master/images/amlNotebookVMsConsole3.png)


