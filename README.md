# Welcome to a hands-on exercise using the **Azure Machine Learning service** and **AI insights** in Power BI Dataflows.

The learning in this exercise is to learn how to create and deploy ML models using the Azure Machine Learning service and then to consume them using **AI insights** in Power BI Dataflows. 


## Prerequisites

1. Need an Azure Subscription for this demo. If you do not have an Azure account, you can sign up for free [here](https://azure.microsoft.com/free/)

2. Need to create a Machine Learning service workspace in an Azure Resource Group

![createworkspace](https://raw.githubusercontent.com/Azure/carprice/master/images/createworkspace.png)

You can find details on creating an AML service workspace [here](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-manage-workspace#create-a-workspace)

3. Save the csv file carprice.csv that is available [here](https://raw.githubusercontent.com/Azure/carprice/master/dataset/carprice.csv)

You can also get the file by downloading a zip of this repository or by cloning this GitHub repository using Git and the following commands:

``git clone https://github.com/Azure/carprice.git``

## Using the NEW **Workspace2 AML Preview Automated machine learning UI**

To learn how to create and deploy a ML model for the carprice dataset using the Azure Machine Learning service **Workspace2 AML Preview Automated machine learning UI** click [here](https://github.com/Azure/carprice/tree/master/ws2preview-automl-ui)

![ws2](https://raw.githubusercontent.com/Azure/carprice/master/images/ws2.png)

## Using the **Azure Portal Automated machine learning UI**

To learn how to create and deploy a ML model for the carprice dataset using the Azure Machine Learning service **Azure Portal Automated machine learning UI** click [here](https://github.com/Azure/carprice/tree/master/automl-ui)

![portal](https://raw.githubusercontent.com/Azure/carprice/master/images/portal.png)

## Using the **Notebook VM**

To learn how to create and deploy a ML model for the carprice dataset using the Azure Machine Learning service **Notebook VM** click [here](https://github.com/Azure/carprice/tree/master/notebooks)

![notebook](https://raw.githubusercontent.com/Azure/carprice/master/images/notebook.png)

## Using the **Visual interface**

To learn how to create and deploy a ML model for the carprice dataset using the Azure Machine Learning service **Visual interface** click [here](https://github.com/Azure/carprice/tree/master/visual-interface)

## Using **AI insights in Power BI**

To learn how to use the carprice ML model to predict the price of a car using **AI insights in Power BI** click [here](https://github.com/Azure/carprice/tree/master/powerbi)

![pbi](https://raw.githubusercontent.com/Azure/carprice/master/images/pbi.png)

At the time of creating this Repo decorating the web service so that it is usable in **AI insights** in a Power BI Dataflow was not available when using the AML service **Visual interface**.  This will not be the case as we move into fall 2019 when this scenario will also work from the **Visual interface**. 

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# Legal Notices

Microsoft and any contributors grant you a license to the Microsoft documentation and other content
in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode),
see the [LICENSE](LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the
[LICENSE-CODE](LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation
may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries.
The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks.
Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents,
or trademarks, whether by implication, estoppel or otherwise.
