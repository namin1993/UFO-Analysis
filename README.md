# UFO's

## Overview
The purpose of this challenge is to create additional filter inputs for our webpage in order to filter out any UFO sighting data that corresponds to our selected date, city, state, country, and shape of the spacecraft.

We modify our javascript file in order to insert the values from user input into an object whose contents we loop through in order to check that each ufo sighting fulfills the conditions in the filter array.

## Results
In  order for the visitor to use the webpage, they must enter their data in the search fields according to the exact format provided in the input box. Not all search fields need a value in order for a search top occur.

### An example for all search fields enetered:
![All_Search_Values_Entered](https://github.com/namin1993/UFO-Analysis/blob/a7216f19704c0bebb1e23bfcd215adc0157c8c6e/Images_For_README/Completely_Filled_Search_Bar.png)

### An example for some search fields enetered:
![Some_Search_Values_Entered](https://github.com/namin1993/UFO-Analysis/blob/a7216f19704c0bebb1e23bfcd215adc0157c8c6e/Images_For_README/Partially_Filled_Search_Bar.png)

The user presses "enter" or "return" on their keyboard. The background javascript will first store the values of each filter into an array in the updateFilters() function. After creating the filter array inside the function, the script will then call the filterTable() function to loop through each value in the filter array in order to match each searchfiled to the filtered table data. It will do this several times depending on how many search values the user entered into the webpage until the final filtered table data contains all of the objects which match all search criteria.

The final result will be a filtered table as seen below:

### An example of a filtered table:
![Filtered_Table](https://github.com/namin1993/UFO-Analysis/blob/a7216f19704c0bebb1e23bfcd215adc0157c8c6e/Images_For_README/Filtered_Search.png)

## Summary
In a summary statement, describe one drawback of this new design and two recommendations for further development.

One drawback for this design is that the "Filter Search" section of the webpage does not evenly line up all search fields. In order to develop this application even further, I would try to improve:
- the bootstrap grid layout of all search fields so that the search fields line up.
- I would change the input box to a dropdown selection for "State" and "Shape" since it's easier for the user to filter the data when they can see the options available instead of guessing. Since all data is from the US, I would also remove "Country" as a search field.
