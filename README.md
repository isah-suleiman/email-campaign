# Email Campaign Performance Analysis

**Executive Summary**  

Every day, we receive countless emails about events, promotions, and newsletters. But have you ever wondered how companies measure the success of these campaigns? This project dives into the email campaign performance of a niche platform designed for DIY creators and readers worldwide.  

The platform offers paid subscriptions, regularly rolls out new features, and hosts monthly online events to keep its audience engaged. Over the past three months, it has run several email campaigns to connect with its audience and drive conversions.  

This analysis focuses on understanding how well these campaigns performed by looking at key metrics like engagement and conversions. The goal is to uncover patterns in audience behavior and find ways to make future campaigns even more effective. By optimizing their email strategy, the platform can strengthen its connection with its community and grow its impact.  

**Problem Statement**  

Email campaigns play a vital role in helping a niche content platform connect with DIY creators and readers around the world. These campaigns are used to promote paid subscriptions, announce new features, and share an exciting calendar of monthly online events. However, it’s unclear how well these emails have performed over the past three months in engaging the audience and driving conversions.  

Without a clear understanding of how recipients interact with these emails, it’s hard to know what’s working and what needs improvement. This makes it challenging to refine strategies and maximize the impact of future campaigns.  

This project aims to analyze the performance of these email campaigns, uncovering valuable insights about audience behavior and identifying practical ways to improve engagement and conversions.  


**Data Description**

This dataset contains information on the performance of email campaigns, collected as part of a data challenge. It includes 34,537 customer records and is accompanied by a data dictionary that provides detailed explanations for each column. The dataset is structured to analyze campaign performance and customer engagement across various dimensions. Below is an overview of the key variables:

1. **Campaign Details:**
   - **Campaign Name:** The name of each email campaign.
   - **Campaign Type:** Categorizes the campaigns into newsletters, events/webinars, promotional campaigns, or lead nurturing.
   - **Conversion Target:** The primary goal of each campaign, such as download, purchase, sign-up, form completion, or website visit.
   - **Date Sent:** The date the campaign was sent to recipients.

2. **Customer Information:**
   - **Client Email:** The email address of the campaign recipient.
   - **Client Segment:** Indicates whether the recipient is a lead or an existing customer.
   - **Country:** The recipient's country of residence.
   - **Country Latitude and Longitude:** Geographical coordinates of the recipient's country.

3. **Device Details:**
   - **Device:** Specifies whether the email was opened on a mobile device or desktop.

4. **Engagement Metrics:**
   - **Clicked:** Indicates if the email received at least one click (value = 1).
   - **Bounced:** Indicates if the email bounced and wasn’t delivered (value = 1).
   - **Opened:** Indicates if the email was opened at least once (value = 1).
   - **Unsubscribed:** Indicates if the recipient unsubscribed from future emails (value = 1).
   - **Conversion:** Indicates if the recipient converted based on the campaign’s goal (value = 1). Conversions include purchases, website visits, form fills, or other defined actions.

