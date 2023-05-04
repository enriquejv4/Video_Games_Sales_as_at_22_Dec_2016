# Video Games Sales as at 22 December 2016

Postgres' database from Video_Games_Sales_as_at_22_Dec_2016.csv

You could find [Video_Games_Sales_as_at_22_Dec_2016.csv](https://www.kaggle.com/datasets/rush4ratio/video-game-sales-with-ratings?resource=download) on Kaggle,
however, we will use a modified version of this csv to fill our postgres database. In this modified version we deleted all cells with 'N/A' from *Year_of_Release* column
and all cells with 'tbd' from *User_Score column*.

In postgres.txt you can see the construction of the postgres' database.

From line 3 to line 64 of postgres.txt we're creating the database's tables. The main table is *videogames* and the rest of the tables are for optimize our database.

In line 67 we're importing Video_Games_Sales_as_at_22_Dec_2016 to *videogames* table.

From line 70 to 83 we're updating secondary tables.

From line 87 to 91 we're dropping updated columns from *videogames* table.

Finally, from line 94 we're crossing our tables to show our final result.
(First 10 rows of 16719)

 name                           | platform | year_of_release | gerne        | publisher | global_sales | developer | rating |
 :-----------------------------:|:--------:|:---------------:|:------------:|:---------:|:------------:|:---------:|:------:|
 Wii Sports                     | Wii      |            2006 | Sports       | Nintendo  |        82.53 | Nintendo  | E      |
 Super Mario Bros.              | NES      |            1985 | Platform     | Nintendo  |        40.24 |           |        |  
 Mario Kart Wii                 | Wii      |            2008 | Racing       | Nintendo  |        35.52 | Nintendo  | E      | 
 Wii Sports Resort              | Wii      |            2009 | Sports       | Nintendo  |        32.77 | Nintendo  | E      | 
 Pokemon Red/Pokemon Blue       | GB       |            1996 | Role-Playing | Nintendo  |        31.37 |           |        |
 Tetris                         | GB       |            1989 | Puzzle       | Nintendo  |        30.26 |           |        |
 New Super Mario Bros.          | DS       |            2006 | Platform     | Nintendo  |         29.8 | Nintendo  | E      |
 Wii Play                       | Wii      |            2006 | Misc         | Nintendo  |        28.92 | Nintendo  | E      |
 New Super Mario Bros. Wii      | Wii      |            2009 | Platform     | Nintendo  |        28.32 | Nintendo  | E      |
 Duck Hunt                      | NES      |            1984 | Shooter      | Nintendo  |        28.31 |           |        |
 
