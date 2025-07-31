# User Profiling for Ad Targeting

##  Project Overview
This project focuses on performing a comprehensive **user profiling analysis** on a dataset of online user behavior and demographic information.  
The primary goal is to segment users into distinct groups (**personas**) based on their characteristics and behavior.  
The insights gained from this segmentation can be used to develop **highly effective, data-driven strategies** for targeted advertising.

---

##  Problem Statement
In today's digital landscape, a one-size-fits-all approach to advertising is often inefficient and leads to a poor return on investment.  
Without a deep understanding of the user base, marketing efforts can be misdirected, resulting in:
- Low engagement  
- Low conversion rates  
- Wasted resources  

The problem is to move beyond generic campaigns and create **personalized, relevant advertisements** that resonate with specific user segments.

---

##  Project Objective
The main objectives of this project are:

1. **Conduct an exploratory data analysis (EDA)** to understand the distribution of key demographic and behavioral variables.
2. **Apply machine learning techniques (K-means clustering)** to segment the user base into meaningful, distinct groups.
3. **Create detailed profiles** for each user segment, identifying their unique characteristics, online behavior patterns, and interests.
4. **Provide actionable insights and recommendations** for targeted advertising campaigns based on the identified user personas.

---

##  Column Dictionary

| Column Name                       | Description                                                        | Data Type |
|-----------------------------------|--------------------------------------------------------------------|-----------|
| **User ID**                       | A unique identifier for each user                                  | int64     |
| **Age**                           | The age range of the user                                          | object    |
| **Gender**                        | The gender of the user                                             | object    |
| **Location**                      | The user's location (Urban, Suburban, Rural)                       | object    |
| **Language**                      | The user's primary language                                        | object    |
| **Education Level**               | The highest education level attained by the user                   | object    |
| **Likes and Reactions**           | The total number of likes and reactions from the user              | int64     |
| **Followed Accounts**             | The number of accounts the user follows                            | int64     |
| **Device Usage**                  | The primary device used by the user                                | object    |
| **Time Spent Online (hrs/weekday)** | The number of hours the user spends online on a weekday          | float64   |
| **Time Spent Online (hrs/weekend)** | The number of hours the user spends online on a weekend          | float64   |
| **Click-Through Rates (CTR)**     | The percentage of ad impressions that resulted in a click          | float64   |
| **Conversion Rates**              | The percentage of clicks that resulted in a desired action         | float64   |
| **Ad Interaction Time (sec)**     | The average time a user spends interacting with an ad              | int64     |
| **Income Level**                  | The user's annual income range                                     | object    |
| **Top Interests**                 | A list of the user's top interests                                 | object    |

---

##  Key Insights

### 1. Demographic and Device Usage
- **Gender:** The user base is nearly balanced, with a slight majority of female users.  
- **Education:** The majority hold **Bachelor's or Master's degrees**, indicating a highly educated base.  
- **Location:** Predominantly **urban and suburban**, with a smaller rural segment.  
- **Device Usage:** **Mobile dominates** (70% use Mobile Only or Mobile + Desktop).  
  > 📢 **Insight:** Ad campaigns should prioritize **mobile optimization**.

---

### 2. Online Behavior and Ad Interaction
- **Time Spent Online:**  
  - Weekday time is more concentrated.  
  - Weekend time is polarized: some disconnect, others have very high usage.  
- **Ad Interaction Time:**  
  - Most users spend **very little time** on ads → ads need to be **quick and impactful**.  
- **Click-Through Rates (CTR):**  
  - CTR ranges widely, with a **central tendency between 0.10 and 0.20**, indicating moderate responsiveness.

---

### 3. User Interests
- The top interests revolve around **lifestyle and creative hobbies** such as:  
  - `Photography`, `Gardening`, `DIY Crafts`  
  >  **Insight:** Content-based advertising aligned with these interests will perform better.

---

##  User Segmentation & Personas
Using **K-means clustering**, five distinct user segments were identified:

### **Cluster 0: Weekend Warriors**
- **Demographics:** Predominantly Male, 25-34 age group, high income ($80k-$100k)  
- **Behavior:** Most active and engaged on weekends, high CTR  
- **Targeting:** Products related to **weekend hobbies and activities**

---

### **Cluster 1: Engaged Professionals**
- **Demographics:** Predominantly Male, 25-34, very high income ($100k+)  
- **Behavior:** Highest engagement across all metrics (likes, reactions, CTR), consistent online time  
- **Targeting:** Premium and high-end products (**most valuable segment**)

---

### **Cluster 2: Low-Key Users**
- **Demographics:** Predominantly Male, 25-34, moderate income ($60k-$80k)  
- **Behavior:** Active online but very low CTR; they consume content but avoid ads  
- **Targeting:** Requires **subtle, content-integrated advertising** rather than direct ads

---

### **Cluster 3: Active Explorers**
- **Demographics:** Predominantly Female, 25-34, moderate income ($60k-$80k)  
- **Behavior:** Most active on weekdays, high CTR but lower likes and reactions  
- **Targeting:** Campaigns with **strong call-to-action during weekdays**

---

### **Cluster 4: Budget Browsers**
- **Demographics:** Predominantly Female, 25-34, lowest income ($0-$20k)  
- **Behavior:** Least engaged across all metrics, low online time, likes, CTR  
- **Targeting:** Focus only if products are **tailored to low-income segments**


### Overall Insight

The core insight is that the user base is not a single, homogeneous group but is composed of five distinct segments with unique demographic profiles, online behaviors, and ad responsiveness. The most valuable segments for high-engagement advertising are the `Engaged Professionals` and `Weekend Warriors`, while the `Active Explorers` and `Low-Key Users` require more nuanced targeting strategies. The `Budget Browsers` are the least engaged and may not be a primary target.

### Recommendations for Targeted Advertising

* **Mobile-First Strategy:** With 70% of the user base using mobile devices, all ad creatives and landing pages must be fully optimized for mobile.
* **Segment-Specific Messaging:** Develop tailored ad campaigns for each persona. For example, for `Weekend Warriors`, run campaigns on weekends and focus on hobby-related products. For `Engaged Professionals`, promote high-end products and premium services with a strong call-to-action.
* **Content-Integrated Ads:** For the `Low-Key Users` segment, consider using more subtle, native advertising or influencer marketing that integrates products naturally into content they already consume, as they are less likely to click on traditional ads.
* **Weekday vs. Weekend Scheduling:** Adjust ad scheduling to align with each segment's behavior. Target `Active Explorers` with promotions during the weekday, while reserving weekend campaigns for the `Weekend Warriors`.
* **Creative Focus:** Given the short ad interaction time, prioritize visually compelling and concise ad creatives that capture attention instantly. Leverage the top interests like 'Photography' and 'Gardening' to create highly relevant and appealing ad content.

### Conclusion

The user profiling and segmentation successfully transformed raw data into a clear, actionable marketing blueprint. By moving beyond generic campaigns and targeting specific user personas, businesses can significantly improve ad effectiveness, boost conversion rates, and maximize their return on investment. This analysis provides the foundation for a smarter, more personalized advertising strategy.

---

## Conclusion
This project demonstrates the power of **user profiling and segmentation** in optimizing ad targeting.  
The findings provide **clear guidance** for designing **personalized** and **effective** advertising strategies.

---
