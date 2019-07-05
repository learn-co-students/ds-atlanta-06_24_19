# Mod 1 Project Instructions


## Congratulations! 

You have just been hired by the Data Science team at Health Data Science for the role of Data Scientist. The team considers data preprocessing a useful skill all data scientist should have. In order to develop data preprocessing skills, new Data Scientist are usually paired and tasked with data preprocessing focused on data cleaning. Along with preprocessing the data, the team requires a presentation showcasing your data visualization skills. In particular, they want visualizations that present findings they can turn into actionable insights for stakeholders. The data set used by the team is the widely used diabetes readmission data set.  

### Why focus on hospital readmission? 
A hospital readmission is an episode when a patient who had been discharged from a hospital is admitted again within a specified time interval. Readmission rates have increasingly been used as an outcome measure in health services research and as a quality benchmark for health systems. Hospital readmission rates were formally included in reimbursement decisions for the Centers for Medicare and Medicaid Services (CMS) as part of the Patient Protection and Affordable Care Act (ACA) of 2010, which penalizes health systems with higher than expected readmission rates through the Hospital Readmission Reduction Program. Since the inception of this penalty, there have been other programs that have been introduced, with the aim to decrease hospital readmission. The Community Based Care Transition Program, Independence At Home Demonstration Program, and Bundled Payments for Care Improvement Initiative are all examples of these programs. While many time frames have been used historically, the most common time frame is within 30 days of discharge, and this is what CMS uses[1].
## Methodology 
Some areas you can look to examine are feature engineering, handlig missing data, and dealing with categorical data. Your team gets to define its own questions about readmission. After forming questions you can then use your knowledge of descriptive statistics(mean, mode, median,etc) and the exploratory data analysis (EDA) process to try and answer those questions. Take a look at the paper below it gives a great explanation of the features used in the data set (pg.3) and how the authors went about handling the data.   
https://www.hindawi.com/journals/bmri/2014/781670/abs/


## Data Source
The data used for the project was obtained from the UCI repository. If you find other useful data on the web you are welcome to include it (but this is not a requirement).  
- **DATA LINK:** https://drive.google.com/file/d/152upD_aPXdpF8WrdAppOKP_uKlqnNtuM/view?usp=sharing
- More data!
  - if you find data you think is helpful, please feel free to ask for instructor help via Slack.


## Deliverables
Your team must prepare a 5 minute presentation that gives the other team members insights as to what features they should focus on to impact hospital readmission. Your presentation must outline the process you went through and use at least 4 meaningful data visualizations to help illustrate your findings. Your team is expected to use git as a collaborative tool for this project to manage version control and history.  No more than 8 slides.

Be prepared to answer questions such as:
- "how did you pick the question(s) that you did?"
- "why are these questions important from a business and/or healthcare perspective?"
- "how did you decide on the data cleaning options you performed?"
- "why did you choose a given method or library?"
- "why did you select those visualizations and what did you learn from each of them?"

## Project Checklist:

 - [ ] Use the data given
   - [ ] Establish naming conventions for variables and datasets
   - [ ] Clean dataset & record parameters used to clean the data
     - [ ] You may use Pandas or Python functions
     - [ ] **Document every step of the cleaning process**
     - [ ] Create **at least two** new features that were not present in the original data sets
 - [ ] Use Pandas and Numpy to generate useful metrics for readmission

 - [ ] Posted to git repository:
   - [ ] A README.md listing project members, goals, responsibilities, and a summary of the files in the repository
   - [ ] At least 10 commits
     - [ ] Must include short, descriptive commit messages
     - [ ] Each project member should commit at least once
   - [ ] A Jupyter notebook targeted to a technical audience that contains
     - [ ] Clean and commented code so an independent party can replicate your analysis and justify your analytical choices
   - [ ] Your final joined and cleaned dataset that was used for analysis
   - [ ] A narrative Jupyter notebook targeted to a non-technical audience that provides:
     - [ ] The purpose of your analysis and why it matters
     - [ ] 4 well annotated visualizations created using Matplotlib/Seaborn
     - [ ] 2 meaningful summary tables
     - [ ] **At least two actionable insights** 
   - [ ] A pdf of no more than 8 slides used in project presentation targeting non-technical audience
     - [ ] Apply consistent and effective formatting to create a “professional” appearance
     - [ ] Write an abbreviated high-level overview of methodology
     - [ ] Justify **at least 2** concrete recommendations 
     - [ ] include exported visualizations from analysis
     - [ ] Target the presentation to a non-technical audience, avoid jargon
     - [ ] Take no more than 5 minutes to present
 
## Specifics:
### This project is in groups
- Group A: Gary Wheeler + Patrick Kim
- Group B: Maia Ngo + Christiaan Defaux
- Group C: Princess Otusanya + Thoa Shook
- Groups are to work independently without outside consulting 
### Timeline

07/05 Friday - Project Assignment 
 - schedule Monday check in with coach
 
07/08 Monday - Check in with coach 
 - review data cleaning
 - provide url of project repository
 - review at least one table/chart
 - review work plan created for how teammates will approach and divide work
 
07/09 Tuesday - Demo presentation with feedback from instructors
 - have polished draft completed
 - have polished version of jupyter notebook completed
 
07/10 Wednesday 
 - afternoon project presentation
 - science fair open to staff and fellow students

### Project Review
If any requirements are missing or if significant gaps in understanding are uncovered, be prepared to do one or all of the following:
 - Perform additional data cleanup, visualization, and/or feature selection 
 - Submit an improved version
 - Meet again for another Project Presentation
 
What won't happen:
 - You won't be yelled at, belittled, or scolded
 - You won't be put on the spot without support
 - There's nothing you can do to instantly blow it
### Citation
[1] Wikipedia contributors. (2019, February 17). Hospital readmission. In Wikipedia, The Free Encyclopedia. Retrieved 22:04, July 4, 2019, from https://en.wikipedia.org/w/index.php?title=Hospital_readmission&oldid=883703655
