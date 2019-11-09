# BabyNames

Baby Names Project
Emily Boling, Phil Lee, Mark Souverville

Data curation
The data we used was pulled from the US social security website.  We downloaded the names by state zip file which resulted in 51 separate txt files (50 states plus DC).  We found it difficult to merge all the files so we found a free software that zipped all the txt files together (txt collector).  Once zipped together, we also had to do some cleaning.  The txt collector added an empty row and a row of gibberish that we had to drop otherwise we had NaNs in our code. We also had to add headers to our data, the pull from uss.gov did not include them.  We also added some data to our dataframe based on some filtering.  We wanted to look at the first initial of each to see which letters were the most popular.  We also wanted to compare USA regions to see if certain areas in the US favored different names so we added in a region column.  Lastly, we wanted to look at various decades to see how trends in names change so we added a decade column to the dataframe.

Questions we wanted to answer:
	What are the most popular baby names from the past 100 years (top 20 for each gender)?
	Are some letters more popular for names?
	How much has the population fluctuated in the past 100 years: what decades have the largest influx?
	Are some names more popular in certain regions of the US?
	Are there more unique female or male names?
	What are the top names from each decade?


Learnings:
We picked a fairly simple data set with only a few columns hoping it would make our analysis more simple.  However, our dataset was large with over 6 million lines.  The large dataset proved to be harder to work with than we expected.  This caused us to look for the quickest ways to do our filtering and addition of desired new columns.  I later found that there was a social security api available, in hindsight it might have been easier to use it.  Our dataset was too large to upload to github, we had to load it as a zip file. This was a good start to the project, with more time and more help I feel we could create something more extensive.
