
## ARM Template for provisioning a Linux Web App with Wordpress connected to Azure Database for MySQL
This template will deploy the following resources into your Azure subscription:

### Azure Web App for Linux (Preview)
### Wordpress 4.7.4 in a Docker container
### Azure Database for MySQL - Basic 50 Compute Unit SKU

Your server will deployed with SSL Disabled as well as firewall rules being set to the full range of 0.0.0.0 - 255.255.255.255.  Feel free to change these afterwards if you'd like to add more security to your DB connection, however note that additional configuration will be necessary for your WordPress site to connect over SSL.

To deploy, make sure to edit the *parameters.json* file and update the fields in ALL CAPITALS specific to your deployment.  No editing is needed of the *template.json* file.  After your *parameters.json* file is edited, save the file and run the following PowerShell command:

```powershell
New-AzureRmResourceGroupDeployment -Name <YOURSITENAME> -TemplateFile c:\<YOURPATH>\template.json -TemplateParameterFile c:\<YOURPATH>\parameters.json
```

To learn more about Azure Database for MySQL, check out our documentation and quick start tutorials [here.](https://docs.microsoft.com/en-us/azure/mysql/overview)  For more information on deploying ARM templates for Azure Web Apps, check [here.](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-template-deploy)

# Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
