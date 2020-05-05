---
title: "Manage your alerts | Microsoft Docs"
description: "Manage alerts in Market Insights."
keywords: "alert management, daily digest, email"
ms.date: 03/27/2020
ms.service: dynamics-365-ai
ms.topic: article
ms.assetid: 7cc0b752-8d1c-4c6f-9f78-81ed326edc7d
author: m-hartmann
ms.author: mhart
ms.custom: dyn365-ai-marketinsights
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365SE
---

# Manage your alerts

[!INCLUDE [market-insights-eos](../includes/market-insights-eos.md)]

(This topic is pre-release documentation and is subject to change.)

We aim to keep your efforts minimal when managing your alerts. After crating your first alert, you can always return to the start page and add more alerts, or edit existing ones.

## Sign in to the app

You can sign in to the app using one of the following accounts: 
- Microsoft account - sends to your organizational email address 
- LinkedIn account - sends to the primary email address of your LinkedIn profile
- Google account - sends to your Google email address

1. Go to [https://alerts.mi.ai.dynamics.com/](https://alerts.mi.ai.dynamics.com/).
2. Select **Sign in** on the top of the page. 
3. Choose which account to sign in with. 
4. Enter your sign-in credentials, usually, this is a combination of an email address and a password.
5. Allow Market Insights alerts to connect with the authenticating service. 
6. Start tracking topics that matter to you or manage existing alerts.

## Create an alert

1. [Sign in](#sign-in-to-the-app) to [https://alerts.mi.ai.dynamics.com/](https://alerts.mi.ai.dynamics.com/).
2. Enter a term or a topic and select the search icon (![Search icon](media/alerts-search-icon.png)). Select **Show advanced** if you want to [specify more details for your search](#tips-on-refining-your-topic).    
--OR--    
Start entering a term and select a suggested entity from the drop-down list. This will create a predefined set of rules for you and focus the results on the selected entity. If you select a suggested entity, the advanced configuration options aren't available.
1. Next to **Email** choose if you want to receive the news **Daily**, or **Weekly**.
2. Select the preferred **Region** for the News and Insights. 
3. Select **Create alert** to finalize your alert.

## Edit an alert

1. [Sign in](#sign-in-to-the-app) to [https://alerts.mi.ai.dynamics.com/](https://alerts.mi.ai.dynamics.com/).
2. In the list of alerts, select the Pen icon ![Edit icon](media/alerts-edit-icon.png) for the alert you want to edit.
3. Apply your changes and select **Update alert**

## Delete an alert

1. [Sign in](#sign-in-to-the-app) to [https://alerts.mi.ai.dynamics.com/](https://alerts.mi.ai.dynamics.com/).
2. In the list of alerts, select the Trashbin icon ![Delete icon](media/alerts-delete-icon.png) for the alert you want to delete.
3. Confirm your deletion.

> [!NOTE]
> You can also **Unsubscribe** from an alert in the email. Unsubscribing deletes the alert too. 

## Tips on refining your topic

Use the **Show Advanced** toggle to refine your search.    
![Show advanced control for Market Insights alerts](media/alerts-show-advanced.png)

Add **more variations of the search term** to *broaden* your search. Example: You want to find generic news about the company Microsoft. When searching for Microsoft, consider searching for the stock ticker symbol (MSFT) too.    
![Add more variations to a search topic](media/alerts-more-terms.png)

Add **inclusions** to *narrow* your search and find news that include both, the search term AND at least one of the terms in box. Example: You want to find news about the Microsoft's Power Platform, but not for generic power platforms.   
![Add terms to appear with the search term](media/alerts-inclusions.png)

Add **exclusions** to *narrow* your search and find news that include the search term but don't include the terms in the box. Example: You want to find news about car industry, but not about car accidents.    
![Add terms to not appear with the search term](media/alerts-exclusions.png)

## Provide feedback about an alert

We'd love to hear what you think about this new service and how we can tailor the experience to your needs. 
You can share your feedback by selecting the **Send feedback** link in the alert email.

### See also

[Manage your alerts](alerts-management.md)    
[How relevancy is determined in alerts](alerts-data-science.md)
