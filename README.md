# Visualizing-NYC311-DataSet
Analyzing Heating Complaint Type of NYC311 DatsSet. This data is New York City’s primary source of government information and
non-emergency services. 311 is a phone number, used in the US, that allows callers to raise a non-emergency complaint. In our analysis, we decided to focus our report around Heating Complaint
Type.
# The Data Set
The 311 DataSet has 52 columns and 912493 rows. Each row represents
a complaint call. The DataSet also has many missing values and could
possibly have duplicate rows.The nyc311 dataset link is https://drive.google.com/file/d/1rdtby7bZPlQODkUr8k2j8C4n7x6oAysR/view?usp=sharing.

# Joining the Dataset with another Dataset
The NYC Population data set was downloaded from
https://data.ny.gov/Government-Finance/Annual-Population-Estimates-forNew-York-State-and/krt9-ym2k. The DataSet has 52 columns and 912493
rows. Each row represents a population of the different states of New York.
The population data set had 5 columns and 3654 rows. The second column was named Geography which we changed into Borough so that it matches our Borough column of nyc311 dataset. In the Borough column we replaced the below data values:
New York County- MANHATTAN
Bronx County- BRONX
Kings County- BROOKLYN
Richmond County- STATEN ISLAND
Queens County -QUEENS
I now filtered the program type column so that we just have the Postcensal Population Estimate and Intercensal Population Estimate. From the new data set we select three columns namely Population, Borough and Year and from the nyc311 data set we select Borough, ComplaintType, IncidentZip, CreatedDate, ClosedDate and Year. For both the dataset we filter out the above mentioned five Boroughs from Fig 3. In addition, we considered the data from 2005 till 2015. We then join both the data sets using Inner Join.

# Tidying the Data Set

Firstly, we remove the missing values from the dataset. After removing the missing values, we’re left with 52 columns and 8293313 rows. We then remove the duplicate rows. Before doing that we need to delete the Unique Key column as even if the same complaint is raised more than once, it’s still going to have different Unique Id. Hence, Inorder to get distinct rows, it is necessary to get rid of the Unique Key column first. Now we’re left with 51 columns and 7455520 rows.

# Aim 
● Which agency receives the most complaints.
● Which month received the most amount of complaints.
● Which was the highest number of complaint types.
● Which Boroughs have the highest number of heating complaints.
● The change in number of calls with the rise of population.

# Run 
1- Download both the datasets and the rmd file and save them in the same folder.
2- Set the directory.
3- Run the file chunk wise.
