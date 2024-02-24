# VTuber Channel, Chat and Superchat Statistics Analysis + Tableau Dashboard

## Purpose of Project
This project serves to showcase my Pandas, Matplotlib and Tableau capabilities by making sense
of VTuber statistics recorded from March 2021 to July 2022. This was all done in a day (24/02/2024).

VTubers have recently emerged as a new type of entertainment for younger people around the
globe. In essence, they are computerised avatars controlled by real people who don a persona
befitting their avatar. VTubers entertain the masses by doing things together with them, from
playing games, to cooking and even simply reading their messages.

Data processing done in this project aims to provide digestable data to a specific VTuber company named
Cover, who operate Hololive (the female branch) and Holostars (the male branch), and its many
variations (generations and locale). This is done in the hope that the company will be better
informed on how to move forward with their expansion and operation plans.

## Data Collection
Data was collected from this (dataset)[https://www.kaggle.com/datasets/uetchy/vtuber-livechat-elements?select=superchat_stats.csv]. Please refer to documentation attached in linked website to further understand variables within the dataset.

## Exploratory Data Analysis
Exploratory data analysis was first done on a Jupyter notebook. From there, it was found that 1358 VTubers from various affiliations were recorded over the span of March 2021 to July 2022.
In addition, 12468 datapoints recording a VTuber's interaction statistics every month and 10942 datapoints recording a VTuber's monthly financial contributions were present in the dataset.

Some alterations had to be done on the dataset before further analysis. While the dataset was very clean, some groups had 'NaN' as a group, which does not give much explaination. As such,
it was altered to 'No Specific Group/Generation' for clarification. Furthermore, there were some Hololive VTubers who despite are officially part of 'Generation 0' were classed as not
belonging to a group (which is fair due to how that generation came to be). Alterations were done to correct the inaccuracy.

Analysis was done to determine the top 10 VTubers by subscriber count for each affiliation and the top 5 VTubers for each generation. Furthermore, deeper analysis was done on Hoshimachi Suisei's and
Sakura Miko's interaction statistics, and on Usada Pekora's financial contributions. This can be seen in vtuber-stats.ipynb.

## Tableau Dashboards
Before using Tableau, raw data was processed to only include necessary columns. This can be seen in tableau-csv-data-prep.ipynb.

While the processed data contained data from all affiliations, a decision was made along the track to only focus on Hololive (and subsequently Holostars) for the sake of time.

Using the processed data, two dashboards were created, all of them featuring filters which change the contents of the dashboard dynamically.

### Dashboard 1: Overall Statistics

Access the dashboard (here)[https://public.tableau.com/app/profile/nicholas.dale/viz/HololiveStats-OverallView/Dashboard1?publish=yes]!

This dashboard features a bubble chart which contains bubbles named after individual Hololive talents, with a bigger bubble indicating more financial contribution done by the talent. Colour was added to indicate
what generation the talent is from.

In addition, a bar chart is available. This bar chart compares subscriber counts between the talents and generations.

### Dashboard 2: Individual Performance

Access the dashboard (here)[https://public.tableau.com/app/profile/nicholas.dale/viz/HololiveStats-IndividualPerformance/Dashboard2?publish=yes]!

This dashboard features a individual talent's superchat statistics (number of superchats received and total superchat money gained), viewer count and status (either a member or just a chatter), and total subscribers
and videos. Each individual can be explored with the available filter. This filter changes the icon on top of it, enabling the user to see the VTuber's avatar.