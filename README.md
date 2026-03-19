# Social Media Engagement Analysis

## Overview

This project analyzes social media engagement data to understand patterns of user interaction on posts. The dataset includes information on likes, shares, comments, posting time, and sentiment. The goal is to identify the most engaging posts and visualize engagement trends using Python, Pandas, Matplotlib, Seaborn, and Plotly.

---

## Dataset

The dataset contains the following columns:
post_id, platform, post_type, post_time, Likes, Comments, Shares, post_day, sentiment_score, engagement

**Key metrics:**

- Likes, Comments, Shares  
- Engagement (calculated as Likes + Comments + Shares)  
- Sentiment score (Positive, Neutral, Negative)  

---

## Data Cleaning & Exploration

Performed initial exploratory data analysis (EDA) using Pandas:

- `df.head()` – View the first few rows of the dataset  
- `df.describe()` – Summary statistics of numeric columns  
- `df.info()` – Check data types and non-null counts  
- `df.isnull().sum()` – Identify missing values  
- `df.duplicated().sum()` – Check for duplicate rows  
- `df.dropna()` – Remove rows with missing data if necessary  
- `df.columns` – View column names  

---

## Analysis & Visualizations

### 1. Distribution Analysis
Visualized the distribution of Likes, Shares, and Comments using:

- Histograms (`sns.histplot`)  
- Boxplots (`sns.boxplot`)
- <img width="1246" height="690" alt="image" src="https://github.com/user-attachments/assets/5ebfefef-cc07-41c4-8529-b1e0cd7bc427" />
- <img width="603" height="433" alt="{CB273A95-3DA9-4F1D-B9F9-DB6BC36FBEBF}" src="https://github.com/user-attachments/assets/3298d3ef-21bf-40f4-9abc-6bfb9a9c624e" />


### 2. Engagement Over Time
- Line plot of total engagement over time to observe trends in post performance.
- <img width="1389" height="590" alt="image" src="https://github.com/user-attachments/assets/44fa111f-89d8-45e1-bcbc-b3fcb40dd1d2" />


### 3. Top Posts
- Top 10 most engaging posts identified using total engagement scores.  
- Bar plots created to visualize the highest performing posts.
- <img width="983" height="527" alt="{77692BA5-8952-46AB-AEE4-9B89C90502F6}" src="https://github.com/user-attachments/assets/3c1b371e-5585-4779-bd34-23a65bef1239" />


### 4. Correlation Analysis
- Correlation heatmap between Likes, Comments, Shares, engagement, and sentiment score to understand relationships between metrics.
- <img width="741" height="668" alt="image" src="https://github.com/user-attachments/assets/a4b11254-4dc4-43c2-84f5-d508fea84e14" />


### 5. 3D Visualizations
**Matplotlib 3D scatter plots:**  
- Engagement across Likes, Comments, and Shares  
- Engagement colored by sentiment (Positive, Neutral, Negative)
- <img width="773" height="660" alt="image" src="https://github.com/user-attachments/assets/69b4bc28-f1bc-41f2-9a7f-759c311ffe5e" />
<img width="798" height="847" alt="image" src="https://github.com/user-attachments/assets/5b89d3b6-aab2-4477-941f-6f1cbcfc6ba2" />


**Plotly 3D scatter plot:**  
- Interactive visualization of engagement by Likes, Comments, and Shares  
- Hover to see exact values  
- Sentiment color-coded for better insights
- fig.write_image("images/newplot.png")
- ![3D Engagement Scatter (Plotly)](newplot.png)
---

## Tools & Libraries

- Python  
- Pandas (data manipulation)  
- Matplotlib & Seaborn (static visualizations)  
- Plotly (interactive 3D visualizations)  

---

## Key Insights

- Some posts achieve extremely high engagement, while most posts have moderate interaction.  
- Likes are generally higher than comments and shares.  
- Engagement trends over time show peaks at specific posting dates.  
- Sentiment plays a role in engagement — posts with positive sentiment often show higher interaction.  
- Correlation heatmaps indicate strong relationships between Likes, Shares, Comments, and total engagement.  

---
## How to Run
1. Clone the repository:  
```bash
git clone https://github.com/Suravipoudel1/SoftGrowTech_task2_social_media_engagement_analysis.git
