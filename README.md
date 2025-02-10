# LEGO-Set-Explorer
Build a custom, interactive tool to help users discover the perfect LEGO set
## about Dataset 
1-set_id:Official LEGO item number

2-name:Name of the LEGO set

3-year:Release year

4-theme:LEGO theme the set belongs to

5-subtheme:Subtheme within the theme

6-themeGroup:Overall group the theme belongs to

7-category:Type of set

8-pieces:Number of pieces in the set

9-minifigs:Number of mini figures included in the set

10-agerange_min:Minimum age recommended

11-US_retailPrice:US retail price at launch

12-bricksetURL:URL for the set on brickset.com

13-thumbnailURL:Small image of the set

14-imageURL:Full size image of the set

## Load and prepare the data:

Your first objective is to load and review the raw LEGO dataset, conduct some basic data prep and profiling, and add calculated columns and DAX measures for analysis.

Tasks: 

1-Connect to the lego_sets CSV file. Remove the minifigs, bricksetURL and thumbnailURL fields, review data types for accuracy, and filter out records with no price, age, pieces or image URL values. How many sets remain? What’s the price range?

2-Create conditional columns for Age Range (“Over 18”, “10 to 17”, “5 to 9”, “1 to 4”) and Price Range (>$500 = “$$$$$”, >$100 = “$$$$”, >$50 = “$$$”, >$25 = “$$”, otherwise “$”)

3-Add measures to calculate the number of distinct sets (Total Sets) and theme groups (Total Groups), as well as the average age (Avg. Age), price (Avg. Price) and pieces (Avg. Pieces)

## Design the report layout & visuals

Your second objective is to design the report layout, add visual elements and filters to the canvas, and configure cross-filtering behavior between visuals.

Tasks:

1- Insert card visuals to show Total Sets, Avg. Pieces and Avg. Price

2- Add slicers to filter based on the theme group, theme and age range

3-Insert a table to show name, set_id, theme, Age Range, Avg. Pieces, Avg. Price and Price Range

4-Add a report section to show details for a selected set, including the name, image, price, year, pieces and age and show placeholder values if multiple sets are selected

5-Edit visual interactions to prevent table selections from filtering the top-level cards

## Add interactive components

Your final objective is to add interactivity to the report using components like parameters, tool tips, bookmark actions and page navigation buttons.

 Tasks:

1- Create a numeric range parameter (Max Price) ranging from 0-850 and incrementing by 5. Add a slicer to the page, and a measure that allows you to filter the table based on the maximum price selected

2- Enable tooltips on the table to display the image of each LEGO set on hover

3- Use bookmarks and button actions to allow users to reset all filters on the page and  customize the format for “on hover” and “on press” states

4- Create a new report page with a decomposition tree visual to analyze Total Sets by category, theme group, theme and name, and add buttons to navigate between pages
















