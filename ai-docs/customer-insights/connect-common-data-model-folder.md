---
title: "Connect Common Data Model data to an Azure Data Lake account | Microsoft Docs"
description: "Work with Common Data Model data in Dynamics 365 Customer Insights using Azure Data Lake Storage."
ms.date: 05/29/2020
ms.service: dynamics-365-ai
ms.topic: "article"
author: m-hartmann
ms.author: mhart
ms.reviewer: adkuppa
manager: shellyha
---

# Connect to a Common Data Model folder using an Azure Data Lake account

This article provides information on how to connect a Common Data Model folder with Dynamics 365 Customer Insights using your Azure Data Lake Storage Gen2 account.

## Important considerations

- Data in your Azure Data Lake needs to follow the Common Data Model standard. Other formats aren't supported at the moment.

- Customer Insights supports Azure Data Lake *Gen2* storage accounts exclusively. You can't use Azure Data Lake Gen1 storage accounts in Customer Insights.

- The Azure Data Lake you want to connect and ingest data from have to be in the same Azure region as Customer Insights environment. Connecting to a Common Data Model folder from an Azure Data Lake in a different Azure region is not supported.

> [!NOTE]
> To know the Azure region of the Customer Insights environment, select the settings icon on the right side of the application header. Then, select **Environments**. In the **Environments** panel you'll find the **Region** value of the environment.

- Data stored in online services, such as Azure Data Lake Storage, may be stored in a different location than where data is processed or stored in Dynamics 365 Customer Insights. By importing or connecting to data stored in online services, you agree that data can be transferred to and stored with Dynamics 365 Customer Insights. [Learn more at the Microsoft Trust Center.](https://www.microsoft.com/trust-center)

## Connect to a Common Data Model folder

1. In Customer Insights, go to **Data** > **Data sources**.

2. Select **Add data source**.

3. Select **Connect to a Common Data Model folder** and select **Next**.

4. Enter a **Name** for the data source and select **Next**.

5. Provide the **Account name**, the **Access key**, and the **Container** for your Azure Data Lake Storage, and select **Next**.
   > [!div class="mx-imgBorder"]
   > ![Dialog box to enter connection details for Azure Data Lake](media/enter-storage-details.png)

6. In the **Select a Common Data Model folder** dialog, select the model.json file that you want to use to import the corresponding entities into Customer Insights. Then select **Next**.
   > [!NOTE]
   > Any model.json file associated with another data source in the instance won't show in the list.

7. You'll get a list of available entities from the selected model.json file. You can review and select from the list of available entities and select **Save**. All of the selected entities will be attached to Customer Insights.
   > [!div class="mx-imgBorder"]
   > ![Dialog box showing a list of entities from a model.json file](media/review-entities.png)

8. After saving your selections, the **Data sources** page opens. You should now see the Common Data Model folder connection as a data source.

> [!NOTE]
> A model.json file can only associate with one data source in the same instance. However, the same model.json file can be used for data sources in multiple instances.

## Edit a Common Data Model folder data source

You can update the access key for the storage account containing the Common Data Model folder you connected to Customer Insights. You may also change the model.json file. To connect to a different container from your storage account, or change the account name, [create a new data source connection](#connect-to-a-common-data-model-folder).

1. In Customer Insights, go to **Data** > **Data sources**.

2. Next to the data source you'd like to update, select the ellipsis.

3. Select the **Edit** option from the list.

4. Optionally, update the **Access key** and select **Next**.

   ![Dialog to edit and update an access key for an existing data source](media/edit-access-key.png)

5. Optionally, choose a different model.json file with a different set of entities from the container.

6. Optionally, you can select additional entities to be attached to Customer Insights. You can also remove any already selected entities if there are no dependencies.

   > [!IMPORTANT]
   > If there are dependencies on the existing model.json file and the set of entities, you'll see an error message and can't select a different model.json file. Remove those dependencies before changing the model.json file or create a new data source with the model.json file that you want to use to avoid removing the dependencies.

   