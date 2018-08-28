---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 1
info:
  title: DataLakeAnalyticsJobManagementClient
  description: creates-an-azure-data-lake-analytics-job-client-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeAnalytics/accounts/{accountName}/StorageAccounts/{storageAccountName}/Containers/{containerName}/listSasTokens
  : post:
      summary: Storage Accounts List Sas Tokens
      description: Gets the SAS token associated with the specified Data Lake Analytics
        and Azure Storage account and container combination.
      operationId: StorageAccounts_ListSasTokens
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountnamestorageaccountsstorageaccountnamecontainerscontainernamelistsastokens-post
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account from which an Azure
          Storage accounts SAS token is being requested
      - in: path
        name: containerName
        description: The name of the Azure storage container for which the SAS token
          is being requested
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      - in: path
        name: storageAccountName
        description: The name of the Azure storage account for which the SAS token
          is being requested
      responses:
        200:
          description: OK
      tags:
      - Stage Account Satokens
---