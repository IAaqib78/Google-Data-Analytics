# Google-Data-Analytics

 




<h1 align="center"> Bellabeat Smart Device Data Analysis</h1>



<h1 align="center" style="font-family:'Segoe UI',sans-serif; color:#66BB6A;">
  
</h1>

<p align="center">
  <img src="bellabeat.jpg" alt="Bellabeat Case Study Banner" style="width:100%; max-width:1200px; height:auto; border-radius:12px; box-shadow:0 0 20px rgba(102,187,106,0.3);">
</p>





<h3 align="center">Developed under <img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/Google_2015_logo.svg" width="80"/> Data Analytics Capstone Project</h3>
<p align="center"><em>Smart device usage insights driving data-informed marketing decisions</em></p>









## **Introduction** 

Welcome to my portfolio-ready case study analyzing smart device usage for Bellabeat, a health-focused tech company that designs wellness products for women. This project was completed using RStudio and R Markdown, and follows the structured data analysis process: Ask, Prepare, Process, Analyze, Share, and Act.

As a junior data analyst, I was tasked with uncovering insights from smart device usage data to help Bellabeat refine its marketing strategy and better understand consumer behavior. This case study simulates a real-world business scenario and demonstrates my ability to work with data, communicate findings, and generate actionable recommendations.

## **Scenario**

Bellabeat is a growing company in the global smart wellness market. Cofounder and Chief Creative Officer Urška Sršen believes that analyzing fitness tracker data can unlock new growth opportunities. I was asked to focus on one Bellabeat product and analyze user behavior using publicly available Fitbit data.

**The goal:**     identify trends in smart device usage and translate those insights into strategic marketing recommendations for Bellabeat.

## **Business Task**

Analyze smart device usage data to answer the following questions:

What are the key trends in smart device usage?

How can these trends apply to Bellabeat customers?

How can these insights inform Bellabeat’s marketing strategy?




<h2 align="center"> Data Sources</h2>

<table align="center" style="max-width:800px;">
  <tr>
    <th align="center" width="220" style="background-color:#1a1a1a;color:#00e6b8;font-size:18px;">Source</th>
    <th align="center" style="background-color:#1a1a1a;color:#00e6b8;font-size:18px;">Description</th>
  </tr>

  <tr>
    <td align="center" style="background-color:#0d1117;color:#e6e6e6;padding:15px;">
      <b>Fitbit Fitness Tracker Dataset</b><br> <i>(CC0: Public Domain via Kaggle)</i>
    </td>
    <td style="background-color:#0d1117;color:#e6e6e6;padding:15px;line-height:1.6;">
      Minute-level activity, sleep, and heart rate data collected from <b>30 consenting Fitbit users</b>. Provides a rich foundation to analyze daily habits, wellness patterns, and behavioral trends, enabling data-driven insights into personal health and lifestyle.
    </td>
  </tr>
</table>




---

<h3 align="center">⚙️ Tech Stack & Tools</h3>

 
  <!-- R Programming -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/r/r-original.svg" width="55" title="R Programming" /> &nbsp;
 
  <!-- RStudio -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rstudio/rstudio-original.svg" width="55" title="RStudio" /> &nbsp;

  <!-- R Libraries -->
  <img src="https://www.r-project.org/logo/Rlogo.png" width="55" title="R Libraries: dplyr, ggplot2, tidyr, readr" /> &nbsp;

  <!-- Git -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="55" title="Git" /> &nbsp;

  <!-- GitHub -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="55" title="GitHub" /> &nbsp;

  <!-- Markdown -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/markdown/markdown-original.svg" width="55" title="Markdown" /> &nbsp;

  <!-- Python -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original-wordmark.svg" width="55" title="Python" />
 

   
 








---



<h2 align="center"> Data Preparation</h2>

<table align="center" style="max-width:900px;">
  <tr>
    <th align="center" width="220" style="background-color:#1a1a1a;color:#00e6b8;font-size:18px;">Step</th>
    <th align="center" style="background-color:#1a1a1a;color:#00e6b8;font-size:18px;">Description</th>
  </tr>

  <tr>
    <td align="center" style="background-color:#0d1117;color:#e6e6e6;padding:15px;">
      <b> Data Import & Exploration</b>
    </td>
    <td style="background-color:#0d1117;color:#e6e6e6;padding:15px;line-height:1.6;">
      Imported multiple CSV files using <b>readr</b> and explored them with <b>dplyr</b> to understand structure, variable types, and overall dataset characteristics.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#0d1117;color:#e6e6e6;padding:15px;">
      <b> Cleaning & Merging</b>
    </td>
    <td style="background-color:#0d1117;color:#e6e6e6;padding:15px;line-height:1.6;">
      Cleaned datasets by removing duplicates, handling missing values, and merged them using <b>distinct()</b>, <b>drop_na()</b>, and <b>inner_join()</b> for a cohesive, unified dataset.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#0d1117;color:#e6e6e6;padding:15px;">
      <b> Data Integrity Verification</b>
    </td>
    <td style="background-color:#0d1117;color:#e6e6e6;padding:15px;line-height:1.6;">
      Verified data structure and consistency, assessing <b>wide vs. long formats</b> and ensuring variables aligned across merged datasets.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#0d1117;color:#e6e6e6;padding:15px;">
      <b> Credibility Assessment</b>
    </td>
    <td style="background-color:#0d1117;color:#e6e6e6;padding:15px;line-height:1.6;">
      Evaluated dataset reliability using the <b>ROCCC framework</b> (Reliable, Original, Comprehensive, Current, Cited) to ensure trustworthy and actionable insights.
    </td>
  </tr>
</table>


---



<h2 align="center"> Analysis & Visualization</h2>

<div align="center" style="max-width:900px; background-color:#111420; color:#e6e6e6; padding:20px; border-radius:12px; line-height:1.7; font-size:16px;">

To uncover meaningful patterns in user behavior, a detailed exploratory analysis was performed using <b>ggplot2</b> and summary statistics. Key relationships examined include:

<ul style="list-style-type:none; padding-left:0;">
  <li> <b>Steps vs. Calories Burned:</b> Visualizations highlighted strong correlations, showing how daily activity translates into energy expenditure.</li>
  <li> <b>Sleep Duration vs. Activity Levels:</b> Analysis revealed how sleep impacts daily activity and overall wellness.</li>
  <li> <b>Daily Intensity vs. User Engagement:</b> Insights into engagement patterns identified peak activity times and adherence to fitness goals.</li>
</ul>

Additionally, <b>summary statistics</b> were calculated to capture average behaviors, identify trends, and reveal usage patterns across the user base. These insights provide a solid foundation for <b>data-driven recommendations</b> and <b>visualization-driven storytelling</b>.

</div>


---















---

## **Key Findings**

Users who took more steps consistently burned more calories

Sleep duration varied widely, but longer sleep correlated with lower activity levels

Most users were moderately active, suggesting potential for targeted engagement strategies

---




---

## **Recommendations**


Based on the analysis, I proposed the following high-level marketing strategies:

Promote Bellabeat’s Time wellness watch to users focused on activity tracking

Emphasize hydration and mindfulness features in the Spring bottle and app

Use personalized insights to drive engagement through Bellabeat’s membership program


---


## **Tools Used**

RStudio

R Markdown

Tidyverse (dplyr, ggplot2, tidyr, readr)

janitor for cleaning column names

GitHub for version control and sharing


---

##  Files in This Repo
- `bellabeat_case_study.Rmd` → Full RMarkdown source code  
- `bellabeat_case_study.html` → Rendered HTML report with plots and insights
- `bellabeat_case_study_insights.pdf` -> pdf version for sharing
- `README.md` → Project documentation 









<p align="center">
  <a href="Case_Study_Report_Bellabeat_Wellness_Insights.html" target="_blank">
    <img src="https://img.shields.io/badge/🚀_Launch_Interactive_Report-%2300c3ff?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=1a1a1a&color=ff0080" 
         alt="Launch Bellabeat Interactive Report" />
  </a>
</p>


















**Contact**

If you’d like to connect or discuss this project further, feel free to reach out via  email:  Kmrtech99@gmail.com
