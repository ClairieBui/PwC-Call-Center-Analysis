# **PwC-Call-Center-Analysis-Power BI Dashboard**
## 📌 **Project Overview**
This project provides a comprehensive data visualization platform for analyzing call center performance. Designed for operational insights and strategic decision-making, these dashboards were created using Power BI, showcasing trends, metrics, and key performance indicators (KPIs) critical for business operations.

## ❓ **Problem Statement**
PwC is struggling to understand itscall center performance. The key areas of concern include:
- **Total Calls** - Monitoring the overall number of calls to assess call center demand.
- **Average Spped of Answers** - Tracking response time to ensure prompt customer service.
- **Total Calls Answered** - Evaluating the efficiency of agents in handling customer inquiries.
- **Total Calls Unanswered** - Tracking inefficient number of calls.
- **Total Calls and Total Resolved by Agent** - Identifying top-performing agents.
- **Total Calls by Answererd (Y/N)** - Measuring call resolution effectiveness.
- **Satisfaction rating** - Assessing customer feedback to enhance service quality.
- **Total Resolved by Topic** - Identifying common customer issues to improve resolution strategies.
- **Total Calls, Total Calls Answered and Total resolved by Month** - Understanding peak call periods to optimize workforce allocation.
- **Total Calls, Total resolved and Total Calls Answered by Day** - Analyzing daily trends to enhance operational efficiency.

The goal was to **explore trends in agent performance, customer satisfaction, and call handling efficiency.**

## 🛠️ **Skills Demonstrated**
- __Power BI__ for data visualization, modeling, and analysis.

## 📊 **Dataset Information**
- **Source**: Excel file containing sales data.
- **Key Columns**:
  - `Call ID`
  - `Agent`
  - `Date`
  - `Time`
  - `Topic`
  - `Answered(Y/N)`
  - `Resolved`
  - `Speed of answer in seconds`
  - `AvgTalkDuration`
  - `Satisfaction rating`

## 🔄 **Data Transformation**
To optimize performance and ensure a well-structured dataset, Power Query was used to transform raw call center data into a star schema model. The model consists of the To optimize performance and structure, **Power Query** was used to transform the raw dataset into a **star schema model**. The original dataset was broken down into:
- **Fact Table**:
  - `Fact_Sales`: Contains call transaction data including `Agent`, `Answered(Y/N)`, `AvgTalkDuration`, `Call Id`, `Date`, `Resolved`, `Satisfaction Rating`, `Speed of Answer in seconds`, `Time`, `Topic`.
- **Additional Time Intelligence Table**:
  - After applying transformations in Power Query and loading the data into **Power BI Desktop**, a dimension table was created:
    - `Dim_Date`: Provides date-based attributes for analysis, including: `Date`, `Day`, `Day Name`, `Day of Week`, `Day Type` fields for date-based analysis.
- **Measure Table**:
  - Measure Table: Contains calculated measures such as:
    -  `Average Talk Duration`

## 📐 **Data Modeling**
Below is the **star schema model** used in this project:
![image](https://github.com/user-attachments/assets/57ae7487-7a32-425d-b67f-450e79d670c3)

## 📈 **Analysis & Visualizations**

**Overview**

![image](https://github.com/user-attachments/assets/2266e182-10a2-411c-968f-e8f15baef0bd)

This dashboard provides insights into call centre operations from January 1st, 2021, to March 31st, 2021, highlighting key performance indicators (KPIs), agent performance, and topic-based resolutions.

1. Key Metrics Overview
   
- **Total Calls**: 5,000 calls were received.
- **Average Speed of Answer**: 67.52 seconds – this suggests potential delays in response times.
- **Total Resolved**: 3,646 calls were successfully resolved, translating to a resolution rate of 72.92%.
- **Calls Answered**: 4,054 calls were handled by agents, meaning 81.08% of all calls were attended to.
- **Calls Unanswered**: 946 calls were missed, which might indicate staffing inefficiencies.

**2. Agent Performance Analysis**
   
- Jim received the highest number of calls (666) but resolved only 488 of them.
- Stewart handled the fewest calls (582) and resolved 424 of them.
- The number of resolved calls per agent remains relatively close, suggesting fairly even distribution in call resolution performance.
- However, Jim, Martha, and Diane have lower resolution rates compared to others, indicating the need for training or process improvements.

**3. Call Answer Rate Analysis**
   
- 81.08% of calls were answered, while 18.92% were missed.
- This suggests room for improvement in call handling capacity, either through increased staffing, better scheduling, or automation (e.g., chatbots, IVR systems).

**4. Resolution Analysis**
- 72.92% of total calls were resolved, meaning 1,354 calls (27.08%) remained unresolved.
- If unresolved calls are leading to customer dissatisfaction, improving first-call resolution (FCR) should be a priority.

**5. Customer Satisfaction**
- The satisfaction rating is 3.40 out of 5, which suggests there is room for improvement in customer experience.
- Factors contributing to low satisfaction could include long wait times, unresolved issues, or agent efficiency.

**6. Topic-Based Call Resolution**
   
- Streaming-related issues had the highest number of resolutions (749), followed by:
- Technical Support (736)
- Payment-Related Issues (729)
- Admin Support (723)
- Contract-Related Issues (709)
  
The high number of streaming and technical support issues suggests that these categories require better troubleshooting processes, self-service options, or proactive customer communication to reduce call volume.

**Trends**

![image](https://github.com/user-attachments/assets/4e6197fc-c1b9-468d-936e-5f388248f474)

1. Monthly Trends Analysis
   
- A downward trend is observed in Total Calls, Total Calls Answered, and Total Resolved from January to March.
- This decline may indicate a seasonal effect, efficiency improvements, or reduced demand over time.

2. Daily Call Distribution
   
- Call volumes remain relatively consistent throughout the week, peaking on Monday and Saturday.
- The number of calls answered and resolved follows a similar pattern, though there might be gaps on peak days.

4. Call Resolution Rate
   
- The total resolution rate appears to be around 72.9%, suggesting that some issues remain unresolved.
- While the call centre is resolving a majority of inquiries, there may be opportunities to improve response efficiency.


## 📌 **Conclusion & Recommendations**

**Conclusion**:
By leveraging Power BI, I uncovered key trends in call center operations, pinpointing areas for improvement in agent performance, customer satisfaction, and call volume management. Implementing these targeted actions can enhance overall efficiency and customer service quality.

**Recommendations**:
- **Enhance Staffing or Automation on Saturdays**: The high rejection rates on Saturdays suggest a shortage of staff. Increasing the number of agents or integrating automated systems could help minimize missed calls and enhance customer satisfaction.

- **Provide Targeted Training for Low-Performing Agents**: Agents such as Jim and Diane may benefit from additional coaching to lower their rejection rates and enhance their call-handling efficiency.

- **Improve Customer Satisfaction Initiatives**: With the current satisfaction rating at 3.40, efforts should focus on faster response times and quicker issue resolutions, particularly in high-demand areas like streaming and technical support.

- **Optimize Monday Staffing**: Since Mondays experience the highest call volume, implementing dynamic scheduling strategies could help manage the influx, leading to lower rejection rates and improved response times.
  
## 🚀 **How to Use This Dashboard**
1. **Download the `.pbix` file** from the repository.
2. **Open Power BI Desktop** and load the file.
3. Use filters and slicers to explore insights interactively.

---
🔗 *For further improvements, feel free to fork this project and contribute!* 🚀

