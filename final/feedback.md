# Feedback on your final

**Final Score: 57/60**

The grading rubric for the final can be found in GitHub: https://github.com/paulboal/hds5210-2023/blob/main/final/final-instructions.pdf

**Functional Requirements**
* 5 points - Uses data from at least two different sources: local file, internet, web service, relational database, AWS S3, etc; and formats: CSV, JSON, database, XML, Excel, etc
* 5 points - Data from multiple sources has to be joined together at least twice
* 5 points - Data is aggregated or pivoted at least twice during the program
* 5 points - Some kind of field-level transformation is performed at least 5 times
* 5 points - The program creates 3 or more data visualizations 
* 5 points - The program serves a theoretical purpose described in documentation, that could potentially do something in healthcare or another industry of interest

**Modularity / Style**
* 15 points - The code is broken up into various functions or classes to make testing and reuse easier

**Documentation and Professionalism**
* 15 points - All functions are documented and notebook cells include annotations and explanations.


**Overall, this was a very strong project. It demonstrated your ability to apply Python skills to data analysis.  There were only a few gaps in the layout and in a couple of operations on your data.  Great work!!**

**In your data cleaning step, I'm curious WHY there might be duplicates in this data.  Shouldn't we expect to only have one row per county/state?  Did you find there were duplicate rows in the data?**

**(-1) You labeled all of the steps you took, but it would have been helpful to have an explanation on WHY you're doing certain things.  Not every step you took was clearly needed or clear about where you were headed.**

**I like all of your data cleansing routines, especially when you were specific about HOW to fill missing data: 0, mean, etc**

**(-1) Your scaler wasn't really a necessary step for the kind of visual/quantitiative analysis you did in this project.  In fact, when you plotted "Total Hospital Beds by State", it made the chart confusing.**

**(-1) When you merge/join two datasets together on columns that aren't unique, you end up duplicating your data.  For example, your "integrated_data" dataframe merged on "state_name" even though some of the data was at the county level and other data had a time dimension to it.  This resulted in duplicate rows.**