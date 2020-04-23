---
title: "Assistant for Dynamics 365 Sales Insights | MicrosoftDocs"
ms.date: 10/31/2018
ms.service: crm-online
ms.custom: 
ms.topic: article
ms.assetid: cf444ca7-3ec1-4939-8710-655190701484
author: udaykirang
ms.author: udag
manager: shujoshi
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
caps.latest.revision: 22
---

# Use assistant to guide customer communications

The assistant (formerly known as Relationship assistant) is part of the new *Sales Insights* suite of features. The assistant keeps an eye on your daily actions and communications, and generates a collection of *action cards* that are displayed prominently throughout the application to provide tailored, actionable insights. The assistant reminds you of upcoming activities; it evaluates your communications and suggests when it might be time to reach out to a contact that’s been inactive for a while; it identifies email messages that may be waiting for a reply from you; it alerts you when an opportunity is nearing its close date; and much more.  

The administrator must enable auto capture before you can try it out. For complete details about prerequisites, how to enable the feature, and how to set it up, see [Configure Assistant](configure-assistant.md).

## How and where the assistant can help you  

 The assistant is designed to deliver the most important and relevant information in relation to what you are doing *right now*. The assistant works by analyzing all of the data at its disposal and generating a collection of action cards, each of which includes a message summarizing what the card is about, plus a set of links for taking action. The assistant sorts the cards by priority and filters them for your current context.  

 When you start your day by signing in to Dynamics 365 Sales, the assistant draws your attention to your most important items and tasks, drawn from all areas of the application.  
  
 ![assistant carousel on a dashboard](media/relationship-assistant-carousel-on-dashboard.png "assistant carousel on a dashboard")  
  
 The figure shows a typical dashboard that includes the assistant carousel. It highlights the following elements:  
  
1. **Action card carousel**: The assistant shows pending action cards here. The most important card is shown on the left, and additional cards may be visible depending on your screen resolution and which view you are using. As you work, dismissing and snoozing cards, additional cards slide in from the right. The figure shows a top-level dashboard, so these cards are drawn from all areas of the site; carousels are also available on individual record views, where the cards are filtered for your specific context.  
  
2. **Action card**: This is a single action card.  
  
3. **Assistant column button**:  select the button to view all available action cards in a vertical, scrollable column. The carousel is hidden when you choose this view.    
4. **Feedback and customization buttons**: These are shown in the upper-right corner of both the carousel and the column views. Use the button on the left to provide feedback about the assistant to Microsoft. Use the button on the right to open your assistant preferences, where you can choose which types of cards you want to see and set options for some of them.  
  
As you drill down into specific records, such as an opportunity or contact, the assistant displays only those cards that are related to the record you are working with. As on the front-page dashboard, the assistant typically opens by showing a carousel, and includes an **Assistant** tab in the center column, which you can open to scroll through all the available cards for the current record.  
  
![Action card example](media/action-card-example-v1.png "Action card example")  
  
Action cards are made up of the following elements, as labeled in the figure:  
  
1. **Main content area**: Shows the title of the record the card refers to, its summary, the card type, and other basic information. Click anywhere in this area (except for on the two buttons) to open the related item, which might be a Dynamics 365 Sales record or an email message .  
  
2. **Actions area**: Provides convenient links that will help you complete whatever type of action the card is recommending. The number (up to two) and types of links provided here vary by card type. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Action cards reference](action-cards-reference.md)  
  
3. **Snooze button**: select the button to hide card temporarily. Snooze time varies by card type. Once the snooze time expires the card will again be visible.  
  
4. **Dismiss button**:  select the button to dismiss card permanently, regardless of whether you have completed the action it recommends.  
  
<a name="Configure"></a>   

## Enable and configure the action cards that are most helpful for you  

 You can customize the assistant by choosing which types of action cards you'd like to see and, for some types of cards, by setting configuration options. To configure the assistant:  
  
1. Sign in to the **Dynamics 365 Sales Hub** app.

2. At the bottom of the site map, select **Change area**, and then select **Sales Insights settings**.

3. Select **Personal settings**, and under **Assistant studio**, select **Insight cards**.

   The **Manage insight cards** page appears with the list of insight cards ordered by status and priority.

   > [!div class="mx-imgBorder"]
   > ![Personal settings for assistant](media/assistant-personal-settings.png "Personal settings for assistant")

**To turn on a card**

- Choose a card that's turned off, and then select **Turn on cards**.  

   Alternatively, you can select the **More options** icon on the card, and then select **Turn on card**. 

   > [!div class="mx-imgBorder"]
   > ![Turn on an insight card](media/assistant-personal-settings-card-turn-on.png "Turn on an insight card")

**To turn off a card**

- Choose a card that's turned on, and then select **Turn off cards**. The card will no longer be displayed for you. 

  Alternatively, you can select the **More options** icon on the card, and then select **Turn off card**. 

   > [!div class="mx-imgBorder"]
   > ![Turn off insight card](media/assistant-personal-settings-card-turn-off.png "Turn off insight card")

   >[!NOTE]
   >- You can select multiple cards and turn off or turn on according to your requirements. 
   >- Some types of cards include additional settings, which are shown in to the right of the check box when available.  
   >- If you are not sure what a listed card or its options do, then try hovering your mouse cursor over the preview button ![Action card preview button](media/action-card-preview-icon.png "Action card preview button") next to the card name see a short description of the card.  
  
  
### See also  

[Configure Assistant](configure-assistant.md)

[Action cards reference](action-cards-reference-v1.md)