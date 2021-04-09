---
title: Data Analysis and Intelligence Blueprint
description: This blueprint shows the ability within Adobe Experience Platform to perform exploratory query and analysis of the data that exists in the data lake.
solution: Experience Platform
kt: 7207
thumbnail: 
exl-id: 3b22dfdd-3fbe-40b3-b798-1ee983723039,a972ea56-d1c8-45da-9044-ed31222a2441
---
# Data Analysis and Intelligence Blueprint

Data Analysis and Intelligence comprises the ability within Adobe Experience Platform to perform exploratory query and analysis of the data that exists in the data lake.

Experience Platform's [!UICONTROL Query Service] allows SQL queries to be performed on the data. [!UICONTROL Data Science Workspace] enables data exploration, data science, and machine learning workloads to be performed on the data. 

In addition, Experience Platform allows connections with third-party SQL clients, interfaces, and Business Intelligence (BI) tools to directly connect to, access and query the data within Experience Platform, using the [!DNL PostgreSQL] protocol.

Certain guardrails apply for the query timeout and for the amount of data that is included in the query result, as noted within the blueprint details.

## Use Cases

* Interactive query and aggregation of data
* Row and column access to ingested data for exploration and validation
* Dashboarding and visualization of data via Business Intelligence tooling

## Applications

* Adobe Experience Platform

## Architecture

<img src="assets/dataexplore.svg" alt="Reference architecture for the Enterprise Data Exploration and Reporting Blueprint" style="border:1px solid #4a4a4a" />

## Guardrails

* 10-minute time limit for interactive queries
* 100-record limit returned in the UI
* 50,000-record limit returned via the SQL connector

## Implementation Steps

1.  Configure datasets and schemas for data ingestion into the data lake.
1.  Ingest data.
1.  Confirm that data is available to [!UICONTROL Query Service] and [!UICONTROL Data Science Workspace] for raw access and query.
1.  Connect Business Intelligence tools and SQL clients to [!UICONTROL Query Service] for visualization, data query, and exploration.

## Related Documentation

* [Adobe Experience Platform Intelligence product description](https://helpx.adobe.com/legal/product-descriptions/adobe-experience-platform-intelligence---product-description.html)
* [[!UICONTROL Query Service] documentation](https://experienceleague.adobe.com/docs/experience-platform/query/home.html?lang=en)