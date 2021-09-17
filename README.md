
#F1 data set analysis 

This project was made as part of the statistical programming coursework, and involved analysing the F1 dataset. 

## Task 1 - Tidy the data

Starting from the `f1` object create a tidy data frame from these data with the following columns:

* `race_name` - The name of the race (character type)
* `round` - Round of the race (integer type, between 1 and 21)
* `date` - Date of the race (date class)
* `driver` - Name of a driver, including first and last name (character type)
* `constructor` - Name of a driver's constructor, i.e. team (character type)
* `position` - Position (place) driver finished in for the race (integer type, `NA` if they did not finish for any reason)
* `points` - Number of points the driver earned for the race (integer type)

Each row of this data frame should represent the result of a driver for a particular race.

Print out 10 rows of this data frame, clearly showing the structure and column types of your answer.

### Additional guidance

* For details on how the race results are reported in the data see the [race result page](https://ergast.com/mrd/methods/results/) on Ergast.

* An optimal solution to this task will not make repeated use of `unnest_longer` and `unnest_wider` - use these sparingly and avoid creating unnecessary columns.



<br/>


## Task 2 - Drivers' Championship

Using the data frame from Task 1, construct a table showing the World Drivers' Championship standings for this F1 season. This table should *resemble* but not be identical to the results available on [Wikipedia](https://en.wikipedia.org/wiki/2019_Formula_One_World_Championship#World_Drivers'_Championship_standings). Your data frame should also have 23 columns: Driver name, finishing position each of the 21 races, and finally thed driver's overall points total for the season. Your data frame should be sorted by points total, you do not need to include any additional logic to handle ties. 

Print out a nicely formatted version of the *complete* table in your rendered document. 


### Additional guidance

* Failure to finish for any reason (did not start, did not finish, disqualified, retired, etc.) should be coded as an `NA`.

* Race finishes and points total should all have an integer type.

* The order of the race columns should follow the chronological order in which the races occurred.

<br />

## Task 3 - Cumulative Constructors

Using the data frame from Task 1 (as a starting point), construct a table that contains the *cumulative* points earned by each of the 10 constructors (teams) at the end of each of the 21 races of the 2019 season. 

For example Mercedes earned 44 points from the Australian Grand Prix, 43 from the Bahrain Grand Prix, and 43 from the Chinese Grand Prix. Therefore the row for Mercedes in this data frame would contain the values 44, 87, 130 for the first three columns, corresponding to these races. 

Your final data frame should have 22 columns: Constructor name and one column for each of the 21 grand prix races. You results should be ordered by the constructors total points at the end of the season.

Print out a nicely formatted version of the *complete* table in your rendered document.

<br />

## Task 4 - Visualization

Design a visualization that shows the performance of *both* drivers and teams over the course of the 2019 F1 season in terms of the points earned toward the drivers' and constructors' Championship standings. This exercise is meant to be purposefully open ended, come up with a visualization that tells a compelling story about this season and use your write up to justify your design choices. Your write up *must* include a discussion of what you are trying to convey as well as how your visualization achieves those goals.

You may use any visualization tools and/or packages you would like as long as your results are reproducible (e.g. I should be able to change the source data and that change would be reflected in the visualization).


