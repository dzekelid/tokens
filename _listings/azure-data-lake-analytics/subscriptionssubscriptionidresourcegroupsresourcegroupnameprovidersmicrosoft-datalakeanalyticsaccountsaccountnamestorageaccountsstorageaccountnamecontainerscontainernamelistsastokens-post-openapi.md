---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Storage Accounts List Sas Tokens
  description: Gets the SAS token associated with the specified Data Lake Analytics
    and Azure Storage account and container combination.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---