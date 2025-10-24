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

<h2 align="center" style="font-family:'Segoe UI', sans-serif; color:#00E676; font-size:28px; text-shadow:0 0 8px rgba(0,230,118,0.6);">
🔑 Key Findings
</h2>

<div align="center" style="max-width:850px; background:linear-gradient(135deg, #0F2027, #203A43, #2C5364); color:#f0f0f0; padding:24px; border-radius:16px; box-shadow:0 0 25px rgba(0,230,118,0.2); font-family:'Segoe UI', sans-serif; line-height:1.8; font-size:17px;">

<ul style="list-style-type:none; padding-left:0; margin:0;">
  <li style="margin-bottom:16px;">
     <b style="color:#00E676;">Step Count & Calories Burned:</b> Users who took more steps consistently burned more calories, highlighting activity as a key driver of energy expenditure.
  </li>
  <li style="margin-bottom:16px;">
     <b style="color:#00E676;">Sleep Patterns & Activity:</b> Sleep duration varied widely, with longer sleep generally correlating with lower daytime activity levels.
  </li>
  <li style="margin-bottom:16px;">
     <b style="color:#00E676;">User Engagement Levels:</b> Most users were moderately active, indicating significant opportunities for <b style="color:#FFD54F;">targeted engagement strategies</b> to boost wellness outcomes.
  </li>
</ul>

<p style="margin-top:20px; font-style:italic; color:#B2DFDB;">
These insights not only reveal behavioral trends but also provide actionable guidance for designing personalized wellness interventions and enhancing user engagement.
</p>

</div>


---




---

<h2 align="center" style="font-family:'Segoe UI', sans-serif; color:#00E5FF; font-size:28px; text-shadow:0 0 8px rgba(0,229,255,0.6);">
 Strategic Recommendations
</h2>

<div align="center" style="max-width:850px; background:linear-gradient(135deg, #1A1F2B, #2C3E50); color:#f2f2f2; padding:24px 28px; border-radius:16px; box-shadow:0 0 25px rgba(0,229,255,0.15); font-family:'Segoe UI', sans-serif; font-size:17px; line-height:1.8;">

<p style="margin-bottom:20px; font-style:italic; color:#B2EBF2;">
Based on the behavioral insights uncovered, the following high-level marketing strategies are recommended to elevate Bellabeat’s product engagement and user experience:
</p>

<ul style="list-style-type:none; padding-left:0; margin:0;">
  <li style="margin-bottom:18px;">
     <b style="color:#00E5FF;">Promote the Time wellness watch</b> to users focused on activity tracking, emphasizing its seamless integration with daily movement goals.
  </li>
  <li style="margin-bottom:18px;">
     <b style="color:#00E5FF;">Highlight hydration and mindfulness features</b> in the Spring bottle and app to appeal to wellness-focused users seeking balance and calm.
  </li>
  <li style="margin-bottom:18px;">
     <b style="color:#00E5FF;">Leverage personalized insights</b> to drive deeper engagement through Bellabeat’s membership program, offering tailored wellness journeys.
  </li>
</ul>

<p style="margin-top:24px; color:#B2EBF2;">
These strategies aim to align product strengths with user needs, fostering long-term loyalty and measurable health outcomes.
</p>

</div>



---


<h2 align="center">🛠️ Tools Used</h2>

<table align="center" style="max-width:900px;">
  <tr>
    <th align="center" width="200" style="background-color:#0f111a;color:#00ffe6;font-size:18px;">Tool</th>
    <th align="center" style="background-color:#0f111a;color:#00ffe6;font-size:18px;">Purpose & Description</th>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/906/906324.png" width="50"/><br><b>RStudio</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Integrated development environment for R. Used for coding, data exploration, and running analytical pipelines seamlessly.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/888/888859.png" width="50"/><br><b>R Markdown</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Combines code, analysis, and narrative in a reproducible format. Ideal for creating professional reports and case studies.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/919/919851.png" width="50"/><br><b>Tidyverse</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Collection of R packages (<b>dplyr, ggplot2, tidyr, readr</b>) used for data manipulation, cleaning, and visualization with elegant syntax.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/1055/1055646.png" width="50"/><br><b>janitor</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Simplifies data cleaning tasks, particularly for cleaning and standardizing column names to ensure tidy datasets.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" width="50"/><br><b>GitHub</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Version control, collaborative development, and sharing of code and reports. Ensures reproducibility and portfolio showcase.
    </td>
  </tr>
</table>


---

<h2 align="center">📂 Files in This Repository</h2>

<table align="center" style="max-width:800px;">
  <tr>
    <th align="center" width="200" style="background-color:#0f111a;color:#00ffe6;font-size:18px;">File</th>
    <th align="center" style="background-color:#0f111a;color:#00ffe6;font-size:18px;">Description</th>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/888/888844.png" width="40"/><br><b>bellabeat_case_study.Rmd</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Full <b>RMarkdown source code</b> containing data import, cleaning, analysis, and visualizations for reproducibility.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/888/888847.png" width="40"/><br><b>bellabeat_case_study.html</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Rendered <b>HTML report</b> with interactive plots and insights, ready for browser viewing and sharing.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/337/337946.png" width="40"/><br><b>bellabeat_case_study_insights.pdf</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      PDF version of the report for sharing offline, summarizing key findings, visualizations, and recommendations.
    </td>
  </tr>

  <tr>
    <td align="center" style="background-color:#111420;color:#e6e6e6;padding:15px;">
      <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" width="40"/><br><b>README.md</b>
    </td>
    <td style="background-color:#111420;color:#e6e6e6;padding:15px;line-height:1.6;">
      Project documentation including methodology, analysis overview, key findings, and tools used.
    </td>
  </tr>
</table>









<p align="center">
  <a href="Case_Study_Report_Bellabeat_Wellness_Insights.html" target="_blank">
    <img src="https://img.shields.io/badge/🚀_Launch_Interactive_Report-%2300c3ff?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=1a1a1a&color=ff0080" 
         alt="Launch Bellabeat Interactive Report" />
  </a>
</p>












<h2 align="center">👩‍💻 Author</h2>

<div align="center" style="max-width:800px; background-color:#111420; color:#e6e6e6; padding:20px; border-radius:12px; line-height:1.7; font-size:16px;">

<img src="https://cdn-icons-png.flaticon.com/512/3135/3135715.png" width="80" style="border-radius:50%; margin-bottom:10px;"/><br>

<b>Aakif Altaf</b>  – Data Scientist & Analytics Enthusiast  

Passionate about transforming raw data into actionable insights, with hands-on expertise in <b>R, Python, SQL, Machine Learning, and Data Visualization</b>. Completed multiple data science and analytics projects, blending technical rigor with storytelling to communicate insights effectively.  

<div style="margin-top:10px;">
  <a href="https://github.com/IAaqib78" target="_blank" style="margin-right:20px;">
    <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="40" title="GitHub"/>
  </a>
  <a href="https://www.linkedin.com/in/aaqib-altaf-94021a146/" target="_blank">
    <img src="https://cdn.worldvectorlogo.com/logos/linkedin-icon-2.svg" width="40" title="LinkedIn"/>
  </a>
</div>

</div>


