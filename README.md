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

**Data Cleaning and Preparation**

For this analysis, I used Power BI to clean and prepare the dataset, leveraging Power Query for exploration and transformation. Here’s a breakdown of the steps I followed:

1. **Ensuring Data Integrity:**  
   I started by checking the dataset for any missing values or outliers. Thankfully, the data was complete and consistent, so no additional imputation or removal of records was needed.

2. **Exploring the Dataset:**  
   Using Power Query, I explored the dataset to understand its structure and the relationships between variables. I reviewed the data types to ensure everything was correctly formatted, such as numbers, text, and dates.

3. **Creating New Columns:**  
   To make the analysis more insightful, I created several conditional columns:  
   - **Clicked Status:** This column categorizes emails as either "Clicked" or "Not Clicked," based on whether recipients interacted with the content.  
   - **Opened Status:** Similarly, this column labels emails as "Opened" or "Not Opened" depending on whether recipients viewed them.  
   - **Conversion Status:** To clarify conversions, I redefined the values in the original "Conversion" column:
     - A `1` now reads as "Converted."
     - A `0` now reads as "Not Converted."

4. **Standardizing and Transforming Data:**  
   - I extracted email domains from the email addresses, which allowed me to analyze engagement and bounce rates by email provider.  
   - I also standardized text columns like campaign names and client segments to ensure consistency throughout the dataset.  

5. **Final Touches:**  
   After cleaning and transforming the data, I verified that everything was ready for analysis. The dataset was now clean, well-organized, and prepared for visualizations in Power BI.

This process ensured that the data was easy to work with and provided meaningful insights into the email campaign performance.

### Analysis, Insights, and Recommendations  

#### **Analysis and Insights**  
1. **Overall Engagement**  
   - A total of **92,337 emails** were sent during the campaign. Out of these, **22,353 emails were opened**, and **2,017 recipients clicked** on the links to take specific actions, like making a purchase or signing up for an event. This resulted in a **conversion rate of 1.38%**.  
   - The bounce rate was impressively low at **0.03%**, indicating that the emails were delivered successfully to most recipients.  

2. **Campaign Performance**  
   - The **Discount Offer for Active Influencers** campaign stood out as the top performer, achieving a **conversion rate of 6.20%**.  
   - While *Events and Webinars* campaigns had the highest **bounce rate (0.06%)**, they also recorded the **lowest unsubscribe rate**, showing strong overall engagement.  
   - Campaigns targeting **desktop users** had a significantly higher **Click-Through Rate (CTR)** and **conversion rate** compared to those targeting other devices, highlighting the effectiveness of desktop-friendly emails.  

3. **Geographic Insights**  
   - The campaign reached audiences in **165 countries**, with **Iceland** standing out for its **100% conversion rate**, suggesting an extremely targeted and successful effort in that region.  

4. **Campaign Types**  
   - **Promotional campaigns** consistently delivered the highest conversion rates, emphasizing the strong appeal of offers and discounts.  

5. **Temporal Trends**  
   - Engagement peaked in **July**, with a **CTR of 2.65%** and a **conversion rate of 1.48%**, before declining in subsequent months.  

#### **Recommendations**  
1. **Improve Device Optimization**  
   - While desktop campaigns performed well, there’s an opportunity to enhance the mobile user experience to close the engagement gap. Focus on creating mobile-optimized designs and ensuring quick loading times for mobile users.  

2. **Expand High-Performing Campaigns**  
   - Campaigns like *Discount Offer for Active Influencers* should be analyzed in detail to replicate their success. Consider using similar strategies, such as personalized discounts or limited-time offers, for other customer segments.  

3. **Focus on Promotional Campaigns**  
   - Allocate more resources to **promotional campaigns**, as they’ve proven to be the most effective in driving conversions. Test different variations of these campaigns to identify what resonates most with your audience.  

4. **Learn from Regional Success**  
   - Investigate why Iceland had such an exceptional conversion rate and replicate those strategies in other regions, particularly those with lower performance. This could involve tailoring the message to specific cultural or demographic preferences.  

5. **Optimize Timing for Campaigns**  
   - Since July showed the highest engagement rates, it’s worth exploring what factors contributed to this success. Timing campaigns around similar conditions—like seasonal trends or major events—could help replicate this performance.  

6. **Enhance Content for Low-Bounce Campaigns**  
   - *Events and Webinars* campaigns had a strong retention rate with the lowest unsubscribe rate. Focus on maintaining the quality of these campaigns while addressing the slightly higher bounce rates by refining email content and targeting strategies.  

### **Tools and Skills Used**  

1. **Power BI**  
   - Utilized Power BI to analyze data, create visuals, and design an interactive dashboard that highlighted key insights.  
   - Leveraged Power Query for data cleaning, exploring the dataset, and creating conditional columns to calculate engagement metrics.  

2. **Data Analysis Techniques**  
   - Measured and analyzed key performance indicators, including open rates, click-through rates (CTR), bounce rates, and conversion rates.  
   - Conducted trend analysis to identify patterns in campaign performance, device usage, and geographical engagement.  

3. **Data Preparation and Exploration**  
   - Explored the dataset to uncover relationships and trends.  
   - Created logical columns to classify data, such as marking "1" in the conversion column as "converted" and "0" as "not converted."  

4. **Communication and Storytelling**  
   - Translated complex findings into easy-to-understand insights tailored to a non-technical audience.  
   - Designed a clear, visually appealing dashboard to effectively communicate performance and recommendations.  

---

### **Conclusion**  

This analysis of the email campaigns provided a clear picture of what worked well and where improvements could be made. For example, promotional campaigns and desktop users stood out as major contributors to high conversion rates, while Iceland demonstrated outstanding engagement with a 100% conversion rate.  

The data also revealed opportunities for optimization, such as refining device targeting strategies and replicating successful campaign approaches across other segments. The low bounce and unsubscribe rates highlighted the overall strength of the email marketing strategy, showing that the content resonated with the audience.  

Through this project, I showcased my ability to analyze data, uncover actionable insights, and present findings in a way that supports decision-making. It was a great opportunity to demonstrate my skills in Power BI, data storytelling, and strategic thinking to help drive business success.
