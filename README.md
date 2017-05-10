## ARM Template for provisioning a Linux Web App with Wordpress connected to Azure Database for MySQL
This template will deploy the following resources into your Azure subscription:

### Azure Web App for Linux (Preview)
### Wordpress 4.7.4 in a Docker container
### Azure Database for MySQL

Your server will deployed with SSL Disabled as well as firewall rules being set to the full range of 0.0.0.0 - 255.255.255.255.  Feel free to change these afterwards if you'd like to add more security to your DB connection, however note that additional configuration will be necessary for your WordPress site to connect over SSL.

If deploying through the **Deploy to Azure** button below, you will have the options to change most of the defaults fairly easily. If deploying through the Azure CLI, it's best that you first clone this repo and edit the **azuredeploy.json** file directly to change the key values to fit your environment.

To learn more about Azure Database for MySQL, check out our documentation and quick start tutorials [here.](https://docs.microsoft.com/en-us/azure/mysql/overview)

# azuredbmysql
[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)
