# YouTube-Trending-Videos-Analysis
Unlocking the Secrets Behind Viral Content
## 🚀 Project Overview

In this project, we dive deep into the world of **YouTube trending videos** in the USA, with the goal of uncovering patterns that predict which videos are likely to trend based on their **titles**. Using **Python**, **PySpark**, and **Tableau**, we've built a machine learning model and crafted beautiful visualizations to shed light on the fascinating world of viral content!

Whether you're a content creator looking to make the next viral video, a marketer aiming to fine-tune your strategies, or a data enthusiast keen on exploring YouTube trends, this project has something for everyone!

## 🔍 Business Problem

**Can we predict the category of a YouTube video based on its title using machine learning?**

Our goal was to use a **Naive Bayes classifier** to categorize videos and explore the factors that make a video popular. By analyzing features like **view counts**, **likes**, and **comments**, we aim to help content creators and marketers understand how videos gain traction and why some categories outperform others.

## 🧠 Analysis Process

### 1. **Data Wrangling & Preprocessing**
   - **Loaded** the dataset using **pandas** and **PySpark** for scalable data processing.
   - **Cleaned** the dataset by dropping unnecessary columns (e.g., `video_id`, `thumbnail_link`), and transforming date columns to a consistent format.
   - Addressed missing data and ensured the quality of video titles by removing unnecessary characters and stop words.
   - We also calculated the **age of each video** (how long it took for a video to trend) and explored correlations between numeric variables.

### 2. **Machine Learning with PySpark**
   - We used **PySpark** to process and analyze large-scale data effectively.
   - **Tokenized video titles**, removed stop words, and created a feature set for the model.
   - **Naive Bayes classifier** was employed to predict the category of videos based on their titles.
   - Model evaluation showed an **accuracy of 74%**, indicating a solid predictive model that can categorize trending videos with high reliability.

### 3. **Tableau Visualizations**
   With the power of **Tableau**, we transformed our data into compelling, interactive visualizations.

   **Key Dashboards:**

   #### 1. Top Performing Channels and Top Categories
   - **Top Performing Channels**: A **treemap** visualization showcasing the most successful YouTube channels, categorized by their respective content categories (e.g., Sports, Entertainment).
   - **Top Categories**: A **bar chart** displaying the most trending categories, such as **Entertainment**, **Music**, and **Gaming**, based on the number of views and videos in each category.
   
     ![image](https://github.com/user-attachments/assets/f589a7c1-f935-4b9a-9ee3-150c99c023ec)

   #### 2. Likes, Views, and Words
   - **Likes vs Views**: A **scatter plot** that shows the correlation between the number of **likes** and **view count** for videos. This helps identify how engagement correlates with video popularity.
   - **Word Cloud**: A **word cloud** of the most common words found in trending YouTube video titles. It reveals which keywords are frequently used in viral content and could be key to increasing engagement.
     ![image](https://github.com/user-attachments/assets/cacf0f41-2194-4f81-9a2b-5b19ad215f52)

## 🛠️ Tools & Technologies

- **PySpark**: For scalable data processing and machine learning.
- **Tableau**: For powerful data visualization and insights sharing.
- **Python Libraries**:
  - **pandas**: For data manipulation and analysis.
  - **NumPy**: For numerical operations.
  - **matplotlib**, **seaborn**: For data visualization.
  - **sklearn**: For implementing machine learning algorithms like Naive Bayes.

## 🎯 Key Insights & Results

1. **Categories That Dominate**: The most trending categories were **Entertainment** and **Music**, with these videos driving the most views, likes, and comments.
2. **Engagement Patterns**: We found a strong relationship between **ViewCount** and **Likes**—but once a video surpassed 10M views, **likes** began to plateau, suggesting a "saturation" point in engagement.
3. **Predictive Power**: Our **Naive Bayes model** accurately predicted the category of a YouTube video 74% of the time, based solely on its title. 
4. **Common Words in Trending Titles**: The word cloud revealed popular keywords such as "Official", "New", and "Music", offering valuable insights into what drives trends.
