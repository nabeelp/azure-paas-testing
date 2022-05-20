# Logic Apps Tests

Folder | Description
--- | --- 
[consumption](consumption/readme.md) | Tests related to the Consumption tier of Logic Apps, also known as multi-tenant Logic Apps, hosted natively in Azure or hosted in an [Integration Service Environemnt (ISE)](https://docs.microsoft.com/en-us/azure/logic-apps/connect-virtual-network-vnet-isolated-environment-overview)
[standard](standard/readme.md) | Tests related to the Standard tier of Logic Apps, also known as single-tenant Logic Apps, hosted on a Windows Standard App Service Plan, or on an [App Service Environment v3 (ASEv3)](https://docs.microsoft.com/en-us/azure/app-service/environment/overview), or on [Azure Kubernetes Service (AKS)](https://docs.microsoft.com/en-us/azure/aks/intro-kubernetes).

For more info on the differences between Consumption (multi-tenant) and Standard (single-tenant) Logic Apps, please review [Single-tenant versus multi-tenant and integration service environment for Azure Logic Apps](https://docs.microsoft.com/en-us/azure/logic-apps/single-tenant-overview-compare).

# Notes

- Investigate if Standard Logic Apps can run on Azure Container Apps
- [DevOps deployment for single-tenant Azure Logic Apps](https://docs.microsoft.com/en-us/azure/logic-apps/devops-deployment-single-tenant-azure-logic-apps)
- [How to run Logic Apps in a Docker container](https://microsoft.github.io/AzureTipsAndTricks/blog/tip311.html)