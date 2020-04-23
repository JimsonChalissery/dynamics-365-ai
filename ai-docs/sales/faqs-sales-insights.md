---
title: "Frequently asked questions for Dynamics 365 Sales Insights | MicrosoftDocs"
description: "Frequently asked questions for Dynamics 365 Sales Insights"
keywords: " "
ms.date: 10/01/2019
ms.service: crm-online
ms.custom: 
ms.topic: article
applies_to:
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
ms.assetid: 848a488e-27ce-41e1-892b-bb8613b5da1c
author: udaykirang
ms.author: udag
manager: shujoshi
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
caps.latest.revision: 01
topic-status: Drafting
---

# Frequently asked questions for Sales Insights

## Language and region support

**What languages are supported now?**<br>
Sales insights supports the following languages:<br>

| Feature | Language supported |
|---------|--------------------|
| Assistant, Assistant studio, Auto capture, Email engagement, Predictive lead scoring, Predictive opportunity scoring, Premium forecasting, Relationship analytics, Sales accelerator, and Who knows whom | Arabic, Basque, Bulgarian, Catalan, Chinese Simplified (PRC), Chinese Traditional (Hong Kong SAR), Chinese Traditional (Taiwan), Croatian, Czech, Danish, Dutch, English, Estonian, Finnish, French, Galician, German, Greek, Hebrew, Hindi, Hungarian, Indonesian, Italian, Japanese, Kazakh, Korean, Latvian, Lithuanian, Malay, Norwegian, Polish, Portuguese (Brazil), Portuguese (Portugal), Romanian, Russian, Serbian (Cyrillic), Serbian (Latin), Slovakian, Slovenian, Spanish, Swedish, Thai, Turkish, Ukrainian, and Vietnamese. |
| Talking points, Notes analysis, and Exchange insight cards in Assistant | Supports only English - United States (en-US) for machine learning models. |
| Activity-content based Auto capture |- For contact suggestions, the body of emails and meetings are analyzed in English and French.<br>- For activity suggestions, the body of emails and meetings are analyzed in English, French, German, Italian, Dutch, and Norwegian. |
| Conversation intelligence (Sales insights application) | Chinese Simplified (PRC), English, French, German, Italian, Japanese, Portuguese (Brazil), and Spanish. |

To learn more, see [Infrastructure availability PDF](https://aka.ms/dynamics_365_international_availability_deck)

**In which region is Sales Insights available?**<br>
Sales insights is available in the following regions:<br>
-    Asia Pacific (APJ)
-    Canada (CAN)
-    Europe, the Middle East, and Africa (EMEA)
-    Great Britain (GBR)
-    India (IND)
-    Japan (JPN)
-    North American (NAM)
-    Oceania (OCE)

## Assistant

**How do I disable teasers?**

To disable, follow these steps:

1. Sign in to the Dynamics 365 Sales Hub app, and go to **Change area** > **Sales Insights settings**.

2. On the site map, select **Overview**.

3. Go to **Teasers** section and toggle the option to disable the teasers.

    > [!div class="mx-imgBorder"]
    > ![Disable teasers](media/disable-teasers.png "Disable teasers")


## Relationship analytics

**What do I need in order to use Relationship analytics?​**<br>
Relationship analytics uses data from Dynamics 365 for Sales. Optionally, it includes data from Exchange Online and LinkedIn InMail with the LinkedIn solution with sync-back enabled. For Exchange data, the graph is built only on user accounts situated in the United States.​

**How do I enable Relationship analytics?​**<br>
Install [!INCLUDE[pn_dynamics_sales_insights](../includes/pn-dynamics-sales-insights.md)] and enable the Relationship analytics feature from  **Settings** > **AI setup**.​

**What is the frequency of KPI updates?​**<br>
KPIs are updated every 24 hours, potentially fewer.​

**What are the signals in relationship health?​**<br>
Relationship health looks at activity, recency, engagement, and sentiment of activities between sellers and customers.​

**Can I configure relationship health?​**<br>
An administrator can influence the relationship health score by changing the weight of activity types and the expected level of communications with customers.

## Predictive lead/opportunity scoring

**What do I need in order to use lead/opportunity scoring?​**<br>
Install [!INCLUDE[pn_dynamics_sales_insights](../includes/pn-dynamics-sales-insights.md)] and use standard lead entity or standard opportunity entity.​

To build a lead score model, a minimum of 40 qualified and 40 disqualified leads are required. 

To build an opportunity scoring model, a minimum of 40 won and 40 lost opportunities are required. 

Verify that the leads and opportunities are created on or after January 01, in the previous year.

**Can I customize the model?​**<br>
You cannot customize the model. The out-of-the-box model automatically selects the features for the model.

**Can I create multiple models for leads/opportunities?​**<br>
No. In this release, you cannot create multiple models. You can create only one model for all leads and one model for all opportunities.

**What is the minimum data required to create a lead/opportunity score model?​**<br>
A minimum of 40 qualified and 40 disqualified leads are required to build a lead score model. 

A minimum of 40 won and 40 lost opportunities are required to build an opportunity scoring model.​

**What is the difference between score and grade?​**<br>
The score is generated by the machine learning model. <br>
The grade is just grouping scores in four buckets that the admin can configure.

## Notes analysis

**What do I need in order to use Notes analysis?​**<br>
Notes analysis requires Office 365.​

**How do I enable Notes analysis?​**<br>
Install [!INCLUDE[pn_dynamics_sales_insights](../includes/pn-dynamics-sales-insights.md)] and enable the Notes analysis feature from **Settings** > **AI setup**.​

**What does Notes analysis look at for the intent?​**<br>
Notes analysis looks at notes and posts on the timeline for the intent that may indicate a record should be created. Notes analysis looks for meeting requests, meetings, tasks, and contacts.

## Talking points

**What do I need in order to use Talking points?​**<br>
Talking points require Office 365 Exchange and a configured server-side sync (SSS) profile (mailbox need not be enabled for SSS).​

**How do I enable Talking points?​**<br>
Install [!INCLUDE[pn_dynamics_sales_insights](../includes/pn-dynamics-sales-insights.md)] and enable the Talking points feature from **Settings** > **AI setup**.​

**What do Talking points look at for the conversation starters?​**<br>
Talking points look at the inbox of the signed-in user for emails from the contact list that includes conversational topics relating to sports, entertainment, and health.​

**How is my privacy protected?​**<br>
User privacy is safeguarded because only emails from the signed-in user's mailbox are shown. Your colleagues won't be able to see those same talking points unless they were also a recipient of that email.​

**How long will it take for results to appear?​**<br>
It takes a few seconds to display the results.​

## Who knows whom

**What do I need in order to use Who knows whom?​**<br>
Who knows whom requires Office 365 Exchange. The graph is built only on user accounts situated in the United States. Geo availability will expand as Sales Insights becomes available in more regions. Server-side sync is required for email introduction requests. ​

**How do I enable Who knows whom?​**<br>
Install [!INCLUDE[pn_dynamics_sales_insights](../includes/pn-dynamics-sales-insights.md)], opt in to Connection insights from the Office 365 admin, and enable the Who knows whom feature from **Settings** > **AI setup**.​

**How long will it take for results to appear?**<br>
The graph requires approximately 24 hours to populate the results for the first time. Subsequent updates take 3-6 days based on new activities included in the graph.​

**​Who will be included in the graph?​**<br>
Everyone in the tenant (in the United States until geo availability expands) will be included in the graph. Administrators have the option to opt out users or DLs, such as C-suite, M&A, finance, and so on. Per user, the self-serve opt-out will be available in the next few months.​

**​How are the connections weighted?**<br>
Connections are weighted by a combination of how well the signed-in user knows the intermediary, and how well the intermediary knows the target contact/lead. Consequently, this means a salesperson might not see the same results as another salesperson because they know different people in the organization.

## Conversation Intelligence

**How long does it take for data updates to reflect in the app?**<br>
The data is refreshed periodically and could take up to 12 hours to reflect. We continue to make improvements to reduce this delay.

**Can sellers (or non-managers) use this app?**<br>
Yes, the application is also available for sellers and can view their conversational insights.

**Is an admin needed to enable the app for my organization?**<br>
Yes. Administrator must configure the application for you to use. If administrator did not configure the application, you can explore the application with the demo data that is provided.

**Which telephony system do you support?​**<br>
The application is independent of telephony systems. If you have stereo call recordings (two-channel stereo), we process them at scale to generate insights​.

**What does the onboarding experience include?​** <br>
As part of the onboarding experience, you must provide the access key to the Azure blob location where you upload your call recording files for processing. You must adhere to standard metadata format (in JSON) of conversation intelligence and upload that along with every call recording file. Apart from this, you must share trackers that you care about along with the competitive brands and products for conversation intelligence to track these words across calls.

**How is the sentiment model built?**<br>
Conversation intelligence transcribes the calls into text and generates sentiment from the text in the conversation.

**I have mono-channel recording files. Can I still use conversation intelligence?​**<br>
No, we DO NOT process mono-channel call recording files. We only support stereo-type call recording files.

**How long does it take to see the results?​**<br>
Conversation intelligence takes a few minutes to process and display the data on the dashboard, depending on the size of the call recording files and format. You must have at least 10 call recording files to process and display the data.

**Do you retain the call recordings?​**<br>
No. The call recordings are deleted as soon as the audio file is processed​.

### See also

[Overview](overview.md)

[Introduction to administer Sales Insights](../sales/intro-admin-guide-sales-insights.md)
