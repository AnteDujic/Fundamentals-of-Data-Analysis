# FUNDAMENTALS OF DATA ANALYSIS | PROJECT | 2021/2022
### AUTHOR: ANTE DUJIC


This repository contains two Jupyter notebooks, done as a project for Fundamentals of Data Analysis module on GMIT, Ireland:
1. cao.ipynb
    - static version
    - interactive version
2. pyplot.ipynb
    - static version
    - interactive version

## cao.ipynb

This notebook gives an overview of how to load CAO points information from the CAO website into a pandas data frame and the comparison of CAO points in 2019, 2020, and 2021. 

### WHAT IS CAO?

[Central Applications Office (CAO)](https://www.cao.ie/) has the purpose to process applications for undergraduate courses in Irish Higher Education Institutions. Students applying for admission to third level education courses in Ireland apply to the CAO rather than to individual educational institutions such as colleges and universities. The CAO then offers places to students who meet the minimum requirements for a course for which they have applied.

### THIS PROJECT

The aim of this project is to collect the data from a website, clear the data and finally analyze and visualize the analysis. I've used Jupyter Notebook for this purpose as it allows the presentation of both the code and the findings in a user friendly interface. 

Before starting the analysis of the data on the CAO website I've done some reasearch to familiarize myself with the data and get the idea of what comparison I would like to do for the mentioned years. 
A few major findings from my research:
1. CAO uploads the points required before the academic year starts and the data contains Round 1 and then Round 2 points. After the year starts the information provided gets changed (same url), and then it contais EOS points and MID points.
    - Round 1 and Round 2 points represent the required points to enter the given course, in first or second round
    - EOS gives the final cut-off points, in other word, the points score achieved by the last applicant being offered a place on that course  [3]
    - MID is the points score of the applicant midwaybetween the highest and the lowest applicant being offered a place  [3]
  
| YEAR | R1 | R2 | EOS | MID |
| :-: | :-: |:-: | :-: | :-: |
| 2019 | &#9744; | &#9744; | &#9745; | &#9745; |
| 2020 | &#9745; | &#9745;  | &#9745;  | &#9745; |
| 2021 | &#9745; | &#9745; | &#9744; | &#9744; |
    
*This CAO practice resulted in the data for each year having different variables and made the comparison for all the years difficult (e.g It was impossible to do a full comparison on 2019 vs 2021). To overcome this issue and get a better data for analysis, I've used the [The Internet Archive](https://web.archive.org/). This allowed me to obtain the data before the changes have been made.*
   
2. There are three different formats the data for each year has been uploaded as - html, pdf and xlxs and each format is structured differently
    - html is the initial data, containing only Round 1 and Round 2 data
    - pdf is the data that is uploaded after the academic year starts and contains only EOS and MID data
    - xlxs is the data that is uploaded after the academic year starts and contains Round 1, Round 2, EOS, MID (and extra data)

| YEAR | DATA FORMAT |
| :-: | :-: |
| 2019 | pdf |
| 2020 | xlxs |
| 2019 | html |

*Due to the data being in different formats, there were different methods used to extract the data from the CAO website. More details on this in the notebook.*


There are 5 questions answered in this notebook:

1. What is CAO?
2. How to load a data from a CAO website?
3. How to clear the data?
4. How to analyse and visually represent the analysis?
5. What is the difference between the data in 2019., 2020. and 2021.?

### HOW TO RUN THIS PROJECT?

1. Download [Anaconda](https://docs.anaconda.com/anaconda/install/windows/)
2. Download [cmder](https://cmder.net/)
3. Run Jupyter Lab or Jupyter Notebook

### HOW TO USE THIS PROJECT?

### ISSUES ENCOUNTERED

Error - not installed
fix
https://rnbeads.org/data/installing_rnbeads.html
After installing ghostscript, we still need to tell R where to find ghostscript. To do so, it is necessary to set adapt your system’s Path variable:
Go to Control Panel → System and Security → System → Advanced System Settings → computer name, domain and workgroup settings → Advanced → Environment Variables
Find the Path variable within System Variables, select it and click on edit.
Add C:\Program Files\gs\gs9.23\bin (or the directory where you installed ghostscript to) to the Path variable. In Windows 10, you can do this by clicking on New and entering the path. In other Windows versions, just append the path to the variable value, seperated by a semicolon.
Restart R

- corrupted pandas!!!
- fixing pandas corrupted camelot!!!
- reinstalled camelot!



## pyplot.ipynb

An overview of the matplotlib.pyplot Python package. This notebook also contains an in-depth explanation of three plots from the matplotlib.pyplot Python package.
