# An Economic Analysis of Virginia's Counties and Independent Cities from 2001 to 2018

Welcome!  You have arrived at an overview of Virginia's economic trends from 2001 to 2018.  Since the 1950s, Virginia has established itself as an economically potent state built on a strong variety of industries, and has embraced the rapid tide of globalization and interstate commerce.  Partly due to its close proximity to Washington, DC, as well as the nationwide shift toward technologically-oriented jobs, Virginia has especially benefited from such changes, prompting citizens as well as businesses from other states to relocate within its limits.

This project will interpret the trends in population, income, and GDP by industry throughout Virginia from 2001 to 2018.  Instead of analyzing Virginia as a whole, we can delve further and examine its individual geographic areas.  For this project, we will define a geographic area as any county or independent city within Virginia.  We do this in order to take into account the impact of geography on predominant industries.  Of course, we can also consider how the rise of an industry in a certain area can affect said area's population and income over time.

### Preparing our Data

Our data can be picked up at the [Bureau of Economic Analysis](https://apps.bea.gov/regional/downloadzip.cfm) as CSV files.  Before we can proceed with our project though, we have to take some steps toward cleaning up our data.  In particular, it must be emphasized that the BEA, for statistical purposes, occasionally labeled one or more cities with an adjacent county.  Therefore, some counties may report higher figures for population, income, and GDP because of those affiliated cities.  For example, while Fairfax City and Falls Church are independent cities, in both of our data sets we notice how the BEA included these two cities under Fairfax County.  Equally important, this should not be conflated with any cities that already present their own separate figures, such as Alexandria and Virginia Beach. 

Additionally, in our GDP by industry data set, we see how some areas did not report any figures for certain industries, regardless of the year.  To resolve this, we can isolate our industries of interest by consolidating some under one description for simplicity purposes.  For instance, we can analyze the trade industry without having to separate wholesale and retail trade from each other.  In doing so, we can add the individual industries together to obtain the total GDP values for each area from 2001 to 2018, and avoid reporting aggregate figures that may not account for certain sectors.

Click [here](https://raw.githubusercontent.com/jvalle58/Valle-DATS-6103-Project-2/main/pop_inc.csv) and [here](https://raw.githubusercontent.com/jvalle58/Valle-DATS-6103-Project-2/main/ind_gdp.csv) to look at the raw pop_inc and ind_gdp data sets, respectively, where you can save these pages as CSV files for reference later.

### Process of Analysis

After cleaning up our data to include only the years 2001 through 2018, we will first examine trends in personal and per capita income in absolute as well as relative figures.  Next, we will turn toward population, and determine the areas with the most significant absolute and relative shifts.  Finally, we will identify which industry constituted the greatest share of total GDP for each area over our time span of interest.  With regard to this last point, we will expand our study toward identifying what relationships, if any, there are between an area's most significant sector and its relative changes in personal income, per capita income, and population from 2001 to 2018.  Using this, we can identify if there any particular industries drawing more people in, or are earning their residents more income, both personal and per capita.

Click [here](https://github.com/jvalle58/Valle-DATS-6103-Project-2/blob/main/DATS%206103%20-%20Individual%20Project%202%20-%20Joseph%20Valle.ipynb) to view the Jupyter Notebook for this project.

### Findings and Conclusions

Overall, one cannot discount the impact that geography plays in shaping the most significant economic sectors of Virginia's counties and cities from 2001 to 2018.  We notice how the areas around the Northern Virginia region especially gained residents over our time span of interest, partly drived by its location within the Washington, DC metropolitan area.  As can be seen from the data, Loudoun County was the only area to more than double its population from 2001 to 2018.  It should be noted that areas such as Spotsylvania and Stafford Counties, both further from the nation's capital, likewise attracted more residents.

On a separate note, in areas with smaller populations, geography can have an equally crucial effect on determining the most influential industries.  We see that especially in the Western Virginia region, where areas like Bath and Buchanan Counties based much of their economies on entertainment and natural resources, respectively.  Both of these are located around the Appalachian Mountains.  On account of their geography, other areas in the Central and Southern Virginia regions tended to focus predominantly on industries such as utilities and manufacturing.

With regard to personal income, based on their trends in population growth, the areas in Northern Virginia also witnessed the biggest gains from 2001 to 2018.  However, trends in per capita income suggested a slightly different story.  While areas in Northern Virginia saw their absolute per capita income grow the most, this was not the case in relative terms.  In one notable case, Fairfax County placed in the top 10 for its absolute gain in per capita income, but ranked in the lowest 10 for its relative gain.  In contrast, areas in the top 10 for their relative gains tended to be in the Eastern Virginia region.  Hence, in the areas that saw more people move in, their rates of growth in terms of their populations exceeded that of their per capita incomes.

In general, areas with higher total GDPs were more likely to have diversified economies, and thus a smaller share of a predominant sector.  This makes sense considering how industries like information, finance, and professional services have accelerated recently, and thus may offer greater avenues for specialization.  In extension to this, specialization opens the door to collaborating with other industries like construction and transportation.  These latter sectors may also shift toward more white-collar occupations as Virginia's economy continues to grow.  Furthermore, economic diversification in an area encourages further urbanization, which subsequently prompts more people to move and find work there.

References for this project are provided below.

### References

Dollar Ticks. (n.d.). Retrieved October 16, 2020, from https://matplotlib.org/3.1.1/gallery/pyplots/dollar_ticks.html

Merge, join, concatenate and compare. (n.d.). Retrieved October 17, 2020, from https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html

Pandas convert column to float. (n.d.). Retrieved October 12, 2020, from https://java2blog.com/pandas-convert-column-to-float/

Pandas.DataFrame.transpose. (n.d.). Retrieved October 17, 2020, from https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.transpose.html

Pandas.Index.rename. (n.d.). Retrieved October 16, 2020, from https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Index.rename.html

Python Pandas : How to convert lists to a dataframe. (2018, September 25). Retrieved October 17, 2020, from https://thispointer.com/python-pandas-how-to-convert-lists-to-a-dataframe/

Regional Economic Accounts: Download. (2019, November 14). Retrieved October 12, 2020, from https://apps.bea.gov/regional/downloadzip.cfm

Replace invalid values with None in Pandas DataFrame. (2013, June 13). Retrieved October 16, 2020, from https://stackoverflow.com/questions/17097236/replace-invalid-values-with-none-in-pandas-dataframe

Renaming columns in pandas. (2012, July 5). Retrieved October 17, 2020, from https://stackoverflow.com/questions/11346283/renaming-columns-in-pandas

Select by partial string from a pandas DataFrame. (2012, July 5). Retrieved October 22, 2020, from https://stackoverflow.com/questions/11350770/select-by-partial-string-from-a-pandas-dataframe

Select rows containing certain values from pandas dataframe. (2016, July 4). Retrieved October 16, 2020, from https://stackoverflow.com/questions/38185688/select-rows-containing-certain-values-from-pandas-dataframe

Slicing multiple column ranges from a dataframe using iloc. (2017, August 31). Retrieved October 16, 2020, from https://stackoverflow.com/questions/45985877/slicing-multiple-column-ranges-from-a-dataframe-using-iloc
