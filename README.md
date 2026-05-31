The objective of this project is to clean and prepare a marketing campaign dataset for analysis.

Rows: 2240
Columns: 29

1.converted dataset to table.

2.all data was in 1 column, data , text to column, delimeter, tab splitted.

3.format auto by width and height

4.blanks:  home, find and select, go to special, blanks,  only income column has blanks, found median value of income by using value(E:E) got 58138 value and ctrl_g special, blank ok enter median value and ctrl+enter to fill to whole blank spaces.
5. no duplicates found.

6.changed Dt_Customer to date form.

7.found outliers like year if birth around 1900 which is irrelevant as there was only few record i deleted those 3 records.

8.removed 2 columns(Z_CostContact, Z_Revenue) of constant values coz this wont show any variation in visual representation.

9.Absurd, Alone, YOLO all these ment single so ctrl+H  using this i replaced all these values to single.

10.created a new column calles age using =YEAR(TODAY())-B2 formula.

11.crated total_children column by using =[@Kidhome]+[@Teenhome].

12.created Total_Spending column using =SUM(J2:O2) .

13.created Total_Purchases column using =P2+Q2+R2.
