# FUNDAMENTALS OF DATA ANALYSIS | PROJECT | 2021/2022
### AUTHOR: ANTE DUJIC

This repository contains two Jupyter notebooks:
1. pyplot.ipynb
2. cao.ipynb

## pyplot.ipynb

An overview of the matplotlib.pyplot Python package. This notebook also contains an in-depth explanation of three plots from the matplotlib.pyplot Python package.

## cao.ipynb

An overview of how to load CAO points information from the CAO website into a pandas data frame. This notevook also contains the comparison of CAO points in 2019, 2020, and 2021.


Error - not installed
fix
https://rnbeads.org/data/installing_rnbeads.html
After installing ghostscript, we still need to tell R where to find ghostscript. To do so, it is necessary to set adapt your system’s Path variable:
Go to Control Panel → System and Security → System → Advanced System Settings → computer name, domain and workgroup settings → Advanced → Environment Variables
Find the Path variable within System Variables, select it and click on edit.
Add C:\Program Files\gs\gs9.23\bin (or the directory where you installed ghostscript to) to the Path variable. In Windows 10, you can do this by clicking on New and entering the path. In other Windows versions, just append the path to the variable value, seperated by a semicolon.
Restart R