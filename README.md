## Title
[Daring to Remember: Journalists in Danger Worldwide](https://ivywang958.github.io/WarAndPeace/)(click to view the webpage)


## Team members
XU Kaiwen  
WANG Ziwei  
LI Mengyu  
SHI Yuning  


## Background and motivation
Jamal Khashoggi, a Saudi journalist known for his criticism on Saudi government, got dismembered
and assassinated at the Saudi Arabian consulate in Istanbul in October. The killing of the dissident
journalist has aroused concern of media outlets worldwide.  
At the time of writing, 52 journalists have been killed this year around the world and 1331 reporters
altogether during the period between 1992 and 2018, according to the [Committee to Protect Journalists](https://cpj.org/). We have scraped the information of those 1324 death records to see
how dangerous it could be to work as a journalist today, in combination with specific case studies
and a face-to-face interview with Dr. Luqiu, a former Chinese war correspondent who covered wars
in Afghanistan and Iraq, Libya and Gaza.


## Quick pointers to key files
### Final Presentation  
Website: [Web page html codes](https://github.com/ivyWANG958/WarAndPeace)  
Class presentation PPT: [Presentation slides](https://drive.google.com/file/d/1HXykljU1yxa2rc7zAWVzolKM6WfaJYhd/view?usp=sharing)(the file is >100M so we upload it to the google drive)  

### Data collection  
Original dataset: [journalists_killed_completed_version.csv](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/journalists_killed_completed_version.csv)  
Data collection phase1: [Data collection-phase 1.ipynb](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/data%20collection-phase%201.ipynb)  
Data collection phase2: ["data collection-phase 2"](https://github.com/kaiwenxu94/Journalists-Killed/tree/master/data%20collection-phase%202)  
We divided the data collection into two phases. The first phase was completed as assignment one(see [data collection-phase 1.ipynb](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/data%20collection-phase%201.ipynb)), which only collected the time, location, organization, type of death and the url attached to each journlist's name, in which further detailed individual information was contained.  
In the second phase, we used splinter to click the urls of 1324 dead journalists one by one to collect detailed individual information such as their job, suspected source of fire, beats covered, etc. We tried to use BeautifulSoup parser at first but no matter how we tried, it failed to extract the information that we wanted from the corresponding html tags, and splinter was the only way left.  
As is shown in the ["data collection-phase 2"](https://github.com/kaiwenxu94/Journalists-Killed/tree/master/data%20collection-phase%202) folder, we divided 1324 items into four parts with 331 each so that the computer could get a rest after scraping 331 items each time(see for example [range(0,331).ipynb](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/data%20collection-phase%202/range(0%2C331).ipynb)). Sometimes splinter just skipped several urls and returned nothing, hence, after scraping for the first time in phase 2, we filtered the missing items and scraped the corresponding pages with splinter again(see for example [cleaned_range(0,331).ipynb](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/data%20collection-phase%202/clean_range(0%2C331).ipynb)). 
The data collection results of the two stages were finally merged into one csv(see [journalists_killed_completed_version.csv](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/journalists_killed_completed_version.csv)). Then we did the data analysis and visualization job.


### Data analysis and visualization  
[Trials on data analysis and visualization](https://github.com/kaiwenxu94/Journalists-Killed/blob/master/data%20analysis%20and%20visualization.ipynb)  
[Collection of interactive diagrams](http://nbviewer.jupyter.org/github/kaiwenxu94/Journalists-Killed/blob/master/Interactive%20Diagram.ipynb)  

### Interview  
[Interview with Dr. Luqiu](https://www.youtube.com/embed/jzmI6e1LB4c)(the file is >100M so we upload it to youtube)  


## References
[Committee to Protect Journalists](https://cpj.org/)  
[Press freedom index](https://en.wikipedia.org/wiki/Press_Freedom_Index) 
