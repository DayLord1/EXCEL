# Data Job Salary Dashboard
<img src="https://github.com/DayLord1/EXCEL/blob/5e445a38dde6c5eb6d29b693ffe3743ed92e94e7/P01_DataJobSalaryDashboard/Pictures/Untitled%20video%20-%20Made%20with%20Clipchamp.gif" width="850" height="550"/>


This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated. 

This dataset comes from an Excel course I completed under the guidance of Luke Barousse on his YouTube channel. The course provided a solid foundation in data analysis using Excel. The dataset includes detailed information on job titles, salaries, locations, and key skills, which are presented here.

### Dashboard File
My final dashboard is in [P01_DataJobSalaryDashboard](https://github.com/DayLord1/EXCEL/blob/bdccc15bbde6011fc674f888b8a53b95b56c8796/P01_DataJobSalaryDashbord/P01_DataJobSalaryDashbord.xlsx)
### Excel Skills Used

The following Excel skills were utilized for analysis:

- **📉 Charts**
- **🧮 Formulas and Functions**
- **❎ Data Validation**

### Data Jobs Dataset

The dataset used for this project contains imaginary real-world data science job information. It includes detailed information on:

- **👨‍💼 Job titles**
- **💰 Salaries**
- **📍 Locations**
- **🛠️ Skills**

## Dashboard Build

### 📉 Charts

#### 📊 Data Science Job Salaries - Bar Chart

<img src="https://github.com/DayLord1/EXCEL/blob/bdccc15bbde6011fc674f888b8a53b95b56c8796/P01_DataJobSalaryDashbord/Pictures/Screenshot%202025-04-06%20162230.png" width="800" height="400" alt="Salary Dashboard Chart1">

- 🛠️ **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 **Design Choice:** Horizontal bar chart for visual comparison of median salaries.
- 📉 **Data Organization:** Sorted job titles by descending salary for improved readability.
- 💡 **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

#### 🗺️ Country Median Salaries - Map Chart

<img src="https://github.com/DayLord1/EXCEL/blob/bdccc15bbde6011fc674f888b8a53b95b56c8796/P01_DataJobSalaryDashbord/Pictures/Maps.gif" width="800" height="400" />

- 🛠️ **Excel Features:** Utilized Excel's map chart feature to plot median salaries globally.
- 🎨 **Design Choice:** Color-coded map to visually differentiate salary levels across regions.
- 📊 **Data Representation:** Plotted median salary for each country with available data.
- 👁️ **Visual Enhancement:** Improved readability and immediate understanding of geographic salary trends.
- 💡 **Insights Gained:** Enables quick grasp of global salary disparities and highlights high/low salary regions.

### 🧮 Formulas and Functions

#### 💰 Median Salary by Job Titles

```
=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)
```

- 🔍 **Multi-Criteria Filtering:** Checks job title, country, schedule type, and excludes blank salaries.
- 📊 **Array Formula:** Utilizes `MEDIAN()` function with nested `IF()` statement to analyze an array.
- 🎯 **Tailored Insights:** Provides specific salary information for job titles, regions, and schedule types.
- **🔢 Formula Purpose:** This formula populates the table below, returning the median salary based on job title, country, and type specified.



### ❎ Data Validation

#### 🔍 Filtered List

- 🔒 **Enhanced Data Validation:** Implementing the filtered list as a data validation rule under the `Job Title`, `Country`, and `Type` option in the Data tab ensures:
    - 🎯 User input is restricted to predefined, validated schedule types
    - 🚫 Incorrect or inconsistent entries are prevented
    - 👥 Overall usability of the dashboard is enhanced

<img src="https://github.com/DayLord1/EXCEL/blob/bdccc15bbde6011fc674f888b8a53b95b56c8796/P01_DataJobSalaryDashbord/Pictures/dropbox.gif" width="425" height="400" alt="Salary Dashboard Data Validation">

## Conclusion 
I created this dashboard to showcase skills I learned throught the course. Utilizing data, this dashboard allows users to make informed decisions about their career paths. Exploring the functionalities to understand how location and job type influence salaries.
