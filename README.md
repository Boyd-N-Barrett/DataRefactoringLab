<h1>Develop Data Pipeline for Hydrological Data Project (2024)


<h2>Description</h2>
I successfully conceptualized, developed, executed, and documented a data pipeline in Python for the Water Protection and Sustainability Branch, Ministry of Water, Land, and Resource Stewardship. I defined data requirements, selected appropriate tools and modules, and built and tested the data pipeline. The pipeline extracts data from multiple sources and creates four feature classes that show the locations of drinking water systems (e.g., wells and aquifers) in British Columbia, Canada.<br />

<br />
Source datasets are stored in the British Columbia Geographic Warehouse (BCGW) and were accessed using a Webservice/API. The script is set to run in Jenkins and automatically updates datasets in the BCGW.<br />

<h2>Languages Used</h2>

- <b>Python</b>

<h2>Environments Used </h2>

- <b>Visual Studio Code</b> (21H2)


<h2>Program walk-through:</h2>

This project was particularly interesting because I used a wide variety of functions and modules that I used. For example, in the first screenshot I show a function that created to compare the schema of two feature classes.
<br />

<p align="center">
Compare the schema of two feature classes: <br/>
<img src="https://imgur.com/ul4WFME.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="left">
In the next screenshot I show the portion of the code that creates the feature classes and add the fields. One of the interesting things about this bit of code is that it pulls information (e.g., feature class name and attribute names and types) from a separate spreadsheet. This enable members of the team who are not capable of using Python to make changes to the feature classes from outside the Python environment.
 
<br />
<p align="center">
Create feature classes and add fields:  <br/>
<img src="https://imgur.com/0JhM6ZL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="left">
The screenshot below shows an example of the Select_Analysis tool and a simple SQL expression. I used this geoprocessing throughout the code to extract features of interest from input layers. 
<br />

<p align="center">
Example of a simple Select-by-Attribute process:  <br/>
<img src="https://imgur.com/OtKIR9Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="left">
In the next screenshot I show an If Else conditional statement. I used these throughout the code to populate fields based on specific criteria. In this instance I populated a field with categorical variables based on the size of the population served by a well or water system. 

This bit of code also includes an UpdateCursor. UpdateCursors establishes read-write access to records in a feature class or table. 
<br />

<p align="center">
If Else statement with UpdateCursor (fun stuff!):  <br/>
<img src="https://imgur.com/Plikydb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="left">
This was a very intersting (and intense) project!

On to the next one
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
