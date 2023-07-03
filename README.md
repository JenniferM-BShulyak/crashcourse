# crashcourse
Analyzing stats of longtime favorite YouTube channel: Crash Course.
## Purpose:
Crash Course is a beloved and powerful educational tool used by teachers and students around the world. Launching on YouTube in 2012, the channel has produced over 40 seasons of courses over topics from biology to film production.

The purpose of this project is to examine the different courses provided to find trends and answer questions regarding course topics that lend to greater success such as:
1. Which genre of courses are the most successful (have the most views, likes, comments...)?
2. Are there any trends in the video statiscs over an individual course's duration (accross its season)?
3. Are there any trends in video statistics through the history of crashcourse?

 ## Methodology:

 ### ETL in Python: 
Extract: Data was pulled from YouTube's API using the channel ID to get a list of the video ids. Then a for loop was constructed to pull the statistics for each video and store the results in a list of dictionaries. A Pandas dataframe was constructed from the list of dictionaries. 

Transform: Data was cleaned using a series of functions to pull out information from the long epsidoe titles such as the course, the episode, and the individual episode title. The parsed information became additiona columns. The published date was converted to datetime format and parsed for the day and time of publication. The duration/length of the videos were converted to seconds. The days seince publication was calculated. Redundant or unuseful columns were removed. 

Load: The final dataframe was loaded as a csv file for use in Tableau.

 ### Data Exploration and Summary in Tableau:

[Tableau Story (Dashbaords)](https://public.tableau.com/app/profile/jennifer.shulyak/viz/CrashCourseAnalysis/Story1?publish=yes)

 ## Analysis:

 [StoryBoard1]!(Images/StoryBoard1.png)

 [StoryBoard2]!(Images/StoryBoard2.png)

 [StoryBoard3]!(Images/StoryBoard3.png)

 [StoryBoard4]!(Images/StoryBoard4.png)

 ## Conclusion: 

