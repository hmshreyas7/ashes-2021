# Data analysis for the Ashes 2021/22 series

## What is this about?
The goal of this project is to analyze and visualize the finer details of the Ashes series and the players/squads participating in it from different angles.

## What are the main files?
As of now, there is only 1 important file: [player_vs_team.ipynb](https://github.com/hmshreyas7/ashes-2021/blob/main/player_vs_team.ipynb) that allows one to compare the batting average of 1 batsman with that of the other top 7 batsmen in his team over the course of his entire Test career.
The third cell contains 5 customizable parameters that can be modified depending on the player of interest. The 'player' and 'team' parameters must be set accurately in the format shown. The exact player name with the correct initials can be found using [Cricinfo Statsguru](https://stats.espncricinfo.com/ci/engine/stats/index.html). The other 3 parameters are only used for customizing the plot and can be set as desired.
Although the purpose of this is to analyze players involved in the Ashes, it can also be used for players from other countries that have played Test match cricket between March 8, 2004 to December 8, 2021.

## What are the dependencies?
* Python 3.10.1
* pandas 1.3.5
* matplotlib 3.5.1
* jupyter-notebook 6.0.1

## Where can the data to reproduce these results be obtained?
The ball-by-ball data for all Test matches between March 8, 2004 to December 8, 2021 was obtained from [Cricsheet](https://cricsheet.org/downloads/tests_csv2.zip). All the individual Test match files were then combined together using an [online tool](https://extendsclass.com/merge-csv.html).

## The purpose of using certain functions in the code is not very clear. Are there any references for these?
The roles of some functions may indeed be hard to figure out at first glance. Some references that might be useful for better understanding are:
1. [Conditional aggregation with groupby and apply](https://stackoverflow.com/questions/17266129/python-pandas-conditional-sum-with-groupby)
2. [Using ravel() to flatten a multi-dimensional array](https://stackoverflow.com/questions/26977076/pandas-unique-values-multiple-columns/26977495#26977495)
3. [Using any() to check if at least 1 "True" element is present](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.any.html)
4. [Setting tick frequency for axes without having to specify upper and lower limits](https://stackoverflow.com/questions/12608788/changing-the-tick-frequency-on-x-or-y-axis-in-matplotlib/58675407#58675407)

Other references which were useful while experimenting are:
1. [Using display() to pretty-print DataFrame](https://stackoverflow.com/questions/26873127/show-dataframe-as-table-in-ipython-notebook#comment90189599_29665452)
2. [Changing the number of rows to display in the Jupyter notebook](https://stackoverflow.com/questions/16424493/pandas-setting-no-of-max-rows)
3. [Dropping all rows before or after an index](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.truncate.html)
4. [Using rolling() to calculate a rolling average](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.rolling.html)