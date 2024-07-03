# Student Performance using Shiny and Flexdashboard

This project focuses on analyzing student performance data using R Shiny and Flexdashboard for interactive data visualization and reporting.

### Overview: 
This dashboard provides a comprehensive view of student performance over the semester. It includes visualizations and summaries to help understand trends and individual performance.

### Key Features: 
- Interactive Dashboards: Created using Shiny and Flexdashboard for dynamic data exploration.
- Summary Statistics: Value boxes showcasing total students, average lab points, and average assignment points.
- Visualizations: Weekly performance analysis with error bars to highlight variations and trends.
- Detailed Scores: A datatable displaying average scores for homeworks and labs for each student.
- Raw Data: A searchable and downloadable table of the raw data with options to filter by student.

## Code Explanation
### Header and Libraries: 
The code starts with the header for the Flexdashboard configuration, setting the format to HTML and including necessary libraries such as Shiny, dplyr, ggplot2, and DT. It also loads the student data and performs initial processing like normalizing scores and extracting semester weeks.

### Summary Section: 
Value boxes are used to display summary statistics like the total number of students and the average scores for labs and assignments. These value boxes are rendered using renderValueBox within the Shiny app.

### Weekly Performance Visualization: 
A bar chart is created using ggplot2 to show the average normalized scores per week, separated by assignment type (homework or lab). Error bars are added to indicate the standard deviation, providing insights into the variability of student performance.

### Student Scores Table: 
The table displays average normalized scores for homework and labs for each student using the gt package. It summarizes the data and provides a clear view of individual performance.

### Data Section: 
This section includes a sidebar with a dropdown menu to select a student and a main panel to display the raw data. The renderDataTable function is used to create an interactive table with options to filter, search, and download the data.

## Website: 
https://aanchal-dusija.shinyapps.io/hw3shiny/
