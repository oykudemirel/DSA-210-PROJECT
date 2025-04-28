# Project Overview
This project aims to investigate the relationship between a movie's release timing and its box office success, examining how these factors influence its chances of receiving award season nominations and wins.


# Motivation
One of the most intriguing aspects of the film industry is the interplay between release timing, box office success, and award season recognition. Why do some movies dominate the box office but fail to win awards, while others achieve critical acclaim despite modest financial performance? Does releasing a movie during awards season increase its chances of winning awards, regardless of box office performance? Do high-grossing movies have a better chance of winning awards, regardless of release timing? What role does the timing of a movie’s release play in its journey to becoming a cultural phenomenon or an award-winning masterpiece? As a movie enthusiast and someone who's interested in data science, this project seeks to unravel these questions by exploring the relationship between a movie’s release timing, its box office performance, and its success during award season. By analyzing publicly available data, I aim to uncover patterns and trends that can shed light on the strategies studios use to maximize both financial returns and critical acclaim. 


# Objectives
1. Examine the Relationship Between Box Office Success and Award Season Recognition
   - Investigate whether higher box office revenue increases a movie’s chances of receiving award nominations and wins.

3. Understand the Impact of Release Timing on Award Season Success
   - Explore whether movies released during awards season (typically November–December) have a higher likelihood of winning awards compared to those released at other times.
   - Assess whether release timing alone can predict award season success, independent of box office performance.

# Data Sources
Box Office Mojo, which tracks box office performance across domestic and international markets. Web Scraping is needed. 

TMDB API will be used for release times and the months will be categorized for further analysis.

I will use Kaggle for Award Show Data: The Oscar Award Dataset, Golden Globe Awards, BAFTA Awards. Such as title, year, if it won an award or not.


# Data Analysis
Download the Award show datasets from Kaggle. Collect box office data from Box Office Mojo. Extract release dates from TMDB.

1. Data Preprocessing:
   - Cleaned and structured datasets from award show data (e.g., Oscars, Golden Globes, BAFTAs), box office data (e.g. Box Office Mojo), and release timing data (TMDB).
   - Collected release timing data using the TMDB API, which has release months. Categorized release timing into seasons (e.g., awards season, summer blockbusters, holiday season, spring).
      
   - Used Web Scraping for Box Office Mojo to get the worldwide box office numbers. Normalized titles then merged datasets by movie title and release year to align movies' release timing and box office performance.
     
   - Cleaned and structured datasets from award show data (e.g., Oscars, Golden Globes, BAFTAs) I filtered the years 2016-2020, then dropped the unnecessary columns so that title, year, and if it won any awards remained in the data. Standardized the columns of each dataset to match each other then merged them, filled the missing values with a 0.
  
   - Merged the TMDB & Box Office Dataset with the merged Award Show Dataset. There's a lot of movies that didnt get nominated so instead of NaN I converted them to 0. 



2. Exploratory Data Analysis (EDA), :
   - Use correlation and regression analysis to explore the relationships between release timing, box office success, and award season success.
     
   - Analyze distributions of box office revenue, award nominations/wins, and release timing across different seasons.
     
   - Visualize trends in award show success according to different release windows (awards season, summer blockbusters, holiday season, spring) and box office performances.
     
   - Investigate whether movies released during peak seasons or with higher box office revenue are more likely to win awards.

   - Create visualizations to represent trends and correlations. Use histograms, boxplots, heatmaps, bar charts, line charts, and scatter plots to illustrate findings.
 

# Hypotheses
- Null Hypothesis (H₀): A movie's release timing (e.g., summer blockbuster season, award season, holiday season, spring) and box office success have no significant impact on its likelihood of receiving award season nominations or wins.
  
- Hypothesis 1 (H1): A movie’s release timing (e.g., summer blockbuster season, award season, holiday season) and box office success significantly influence its chances of receiving award season nominations or wins.


