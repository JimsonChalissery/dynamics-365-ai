---
title: "Entities in Dynamics 365 Customer Insights | Microsoft Docs"
description: "View ingested data on the Entities page in Dynamics 365 Customer Insights."
ms.date: 04/16/2020
ms.reviewer: mukeshpo
ms.service: dynamics-365-ai
ms.topic: "get-started-article"
author: m-hartmann
ms.author: mhart
manager: shellyha
---

# Entities in Customer Insights

After [configuring your data sources](pm-data-sources.md), go to the **Entities** page to evaluate the quality of the ingested data. In Dynamics 365 Customer Insights, entities are considered datasets. Multiple capabilities of Customer Insights are built around these entities. Reviewing them closely can help you validate the output of those capabilities.

The **Entities** page lists entities and includes several columns:

- **Name**: The name of your data entity. If you see a warning symbol next to an entity name, it means that the data for that entity didn't load successfully.
- **Source**: The type of data source that ingested the entity
- **Created by**: Name of the person who created the entity
- **Created**: Date and time of the entity creation
- **Updated by**: Name of the person who updated the entity
- **Last updated**: Date and time of the last update of the entity
- **Last refresh**: Date and time of the last data refresh

## Exploring a specific entity's data

Select an entity to explore the different fields and records included within that entity.

> [!div class="mx-imgBorder"]
> ![Select an entity](media/data-manager-entities-data.png "Select an entity")

- The **Data** tab is selected by default and shows a table listing details about individual records of the entity.

> [!div class="mx-imgBorder"]
> ![Fields table](media/data-manager-entities-fields.PNG "Fields table")

- The **Fields** tab shows a table to review details for the selected entity, such as field names, data types, and types. The **Type** column shows Common Data Model associated types, which are either auto-identified by the system or [manually mapped](pm-map.md) by users. These are semantic types that can differ from the attributes' data types—for example, the field *Email* below has a data type *Text* but its (semantic) Common Data Model type might be *Email* or *EmailAddress*.

> [!NOTE]
> Both tables show only a sample of your entity's data. To view the full data set, go to the **Data sources** page, select an entity, select **Edit**, and then view this entity's data with the Power Query editor as explained in [Data sources](pm-data-sources.md).

To learn more about the data ingested in the entity, the **Summary** column provides you with some important characteristics of the data, such as nulls, missing values, unique values, counts, and distributions, as applicable to your data.

Select the chart icon to see the summary of the data.

> [!div class="mx-imgBorder"]
> ![Summary symbol](media/data-manager-entities-summary.png "Data summary table")

### Next step

See the [Unify](pm-configure-data.md) topic to learn how to *map*, *match*, and *merge* the ingested data.
