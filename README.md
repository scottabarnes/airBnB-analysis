# 1-AirBnB-Analysis
Link to notebooks:
- Notebooks can be reviewed on [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/github/scottabarnes/airBnB-analysis/tree/main/nbs/)

Overview & objectives:
- This project was focused on performing exploratory data analysis looking at the impact of the global pandemic on AirBnB listings in London 
- The project looked at data relating to 1) listing pricing, 2) property availability and 3) stay offerings and observed changes before, during and after the lockdown months in an attempt to understand the impact of the pandemic

Folder layout:
- The notebooks for the project are stored in the nbs folder
- Within the nbs folder there is a Data Processing and Data Analysis notebook 

Files used in analysis:
- The data used in the analysis was obtained from Inside AirBnB: http://insideairbnb.com/get-the-data.html
- 12 periods of data were taken, from August 2019 to August 2020 (data scraped from July 2020 is not available on the site)
- The compressed calendar and listing files were the main files used in the analysis 

Summary of results:
1. Pricing
    - The analysis identified an increased proportion of hosts offering last minute discounts in the months of lockdown in London
    - It was found that hosts with more properties were more likely to significantly discount their properties than hosts with less
2. Property availability 
    - The analysis identified a decrease in the proportion of available properties around the months of lockdown in London
    - The analysis also identifed a reduction in the overall volume of properties listed on AirBnB since June 2020
3. Stay type
    - The analysis identified a recent change in the volume of properties with a minimum stay of 4 - 6 nights vs. 7 + nights
    - Before April 2020 there wre more listings with the shorter minimum stay, but after that point the longer minimum stay became more common  
 

Challenges:
- Size of data files used 
    - The data files used for the analysis were quite large and it was not possible to hold several periods of data in memory on a local machine 
    - The solution to this was to read in the file required, perform aggregations, then delete and iterate onto the next period 
    
Libraries used:
- The key libraries used were:
    - Numpy and Pandas for data wrangling 
    - Matplotlib and Plotly for data visualisation 
    - os for directory management 
