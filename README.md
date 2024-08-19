# CryptoClustering

# Notes: started off by renaming the source file, as directed.  Renamed with mv on terminal to get used to using interface instead of GUI on desktop.

# First step (already provided) was to pull in the information from the provided csv file and set the column to “coin_id”.

# Second step (not in instructions but done to understand the information): Displayed the information in the imported data frame, named “market_data_df” and added a few other ways to inspect the data (determine that they are all floats and their length, etc . . . )

# Third – per the instructions we used the StandardScaler function.  And the idea here was to take data that had some moving wildly (bitcoin-cash) and some with very small changes (e.g. ripple) being put on the same scale around a standard mean so that the movements by the ones with big numbers don’t overwhelm any other assessment of the data and render it a proxy for information about which has the largest numbers.

# Fourth – we’re going to use K-Means.   Modeled this on the customer agglomeration we did under 11-2-7 Student Learning (solved version).  Only change was to automatically cycle it through 1-11 and created the list with the inertira so we can find the ‘elbow’ joint

# Fifth – we ran the code and obtained the “elbow” we were looking for.  It’s pretty clear that 5 is the right cutoff with every little inertia after that number. 

# Six – ran the K-means with 5 and split the coins into 5 categories (0, 1, 2, 3, 4) which are added as a column.

# Seventh – made a rainbow chart.  

# Eighth – not part of instructions – played around with different x/y information to see if different shapes manifested themselves
