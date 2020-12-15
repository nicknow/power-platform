---
title: Set up exporting to Application Insights | Microsoft Docs
description: About setting up exporting to Application Insights from the Power Platform admin center
services: powerapps
author: jimholtz
ms.service: power-platform
ms.component: pa-admin
ms.topic: conceptual
ms.date: 12/08/2020
ms.author: jimholtz
search.audienceType: 
  - admin
search.app:
  - D365CE
  - PowerApps
  - Powerplatform
  - Flow
---
# Set up exporting to Application Insights  

## Prerequisites

1. Ensure that you have an [Application Insights environment](https://docs.microsoft.com/azure/azure-monitor/app/create-new-resource) set up for receiving the data as well as the [environment](environments-overview.md) with a database. 
   - You must have one of these - contributor, writer or admin rights - for the Application Insights environment created.
   - The Application Insights environment must be unique for an environment/tenant. Note that Application Insights out of box reports will not function correctly if a single Application Insights has multiple environments data.
2. The data export setup in the [Power Platform admin center](https://admin.powerplatform.microsoft.com/) will require one of these roles - Power Platform Service admin, Dynamics 365 admin, or Microsoft 365 Global admin. 

## Set up export to your Applications Insights environment from the Power Platform admin center

1. In the Power Platform admin center, select **Data Export** > **New data export**.

   > [!div class="mx-imgBorder"] 
   > ![Data export](media/data-export.png "Data export")

2. Select **Export to Application Insights**. 

   > [!div class="mx-imgBorder"] 
   > ![Data export to Application Insights](media/data-export-application-insights.png "Data export to Application Insights")

3. Search for the environment that you will set up for the Application Insights data export setup. You can choose to filter based on the environment type.

   > [!div class="mx-imgBorder"] 
   > ![Select an environment type](media/data-export-application-insights-select-environment-type.png "Select an environment type")

   Select **Save** after choosing the environment.

   > [!div class="mx-imgBorder"] 
   > ![Select an environment](media/data-export-application-insights-select-environment.png "Select an environment")

4. Choose the Azure subscription, Resource Group, and Application Insights environment, and then select **Create**. You must have one of the following rights - contributor, writer or admin - to the Application Insights environment. Typically, a production environment/tenant will map to one Application Insights environment. 

   > [!div class="mx-imgBorder"] 
   > ![Data export Application Insights details](media/data-export-application-insights-details.png "Data export Application Insights details")

5. The data export connection should now be set up. In the next 24 hours, data will start being exported to your Application Insights environment.

   > [!div class="mx-imgBorder"] 
   > ![Data export success](media/data-export-application-insights-success.png "Data export success")

6. To stop the data export to Application Insights, select **Delete export**. You can set up a new connection whenever you decide to restart the data export.

   > [!div class="mx-imgBorder"] 
   > ![Delete export](media/data-export-delete.png "Delete export")

## Regional Availability 

|Zone  |Public Preview availability  |
|---------|---------|
|Canada     | Jan 2021        |
|EMEA     | Jan 2021        |
|North America     | Jan 2021        |
|Germany  | Azure Dependencies        |
|France     | March 2021        |
|South America     | Jan 2021        |
|Asia Pacific     |  Jan 2021       |
|Japan     |  Jan 2021       |
|UK     | Jan 2021        |
|OCE     | Jan 2021        |
|India     | March 2021        |
|South Africa (ZAF)     | Azure Dependencies        |
|UAE     | March 2021        |
|Switzerland (CHE)     | Azure Dependencies        |


