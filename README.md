# UFOs
## Overview of Project 
This project requires the creating a webpage that displays data on UFO sightings.  There is a large number of sightings and multiple filters are going to be needed so that it is meaningful to the user.

## Resources
Data Sources:  data.js
Software: JavaScript, Bootstrap, d3.js, and Visual Studio Code

## Results

![UFO Finder screenshot](https://github.com/BlazeMedina/UFOs/blob/main/static/images/Screenshot%202023-03-16%20154826.png)

After creating the UFO Finder webpage layout, the filters needed to be created and the corresponding data needed to be displayed.  Created user input areas for date, city, state, country, and shape.  In app.js, created filters for each input and utilized an event handler to call the function 'updateFilters' when there is a change in the user input area.  The 'updateFilters' function stores the value of the updated user input and calls the 'filterTable' function.  The 'filterTable' function loops through all the filters and keeps any data that matches the user inputs.  Then the 'buildTable' function is called and just the filtered data is displayed on the webpage in the table body.

To use the search criteria to filter the data, the user needs to enter their criteria in the appropriate field and then press ENTER.  To further filter the data, enter another criteria on another filter and press ENTER.

## Summary
One drawback to this design is that users must use all lower cases when entering in the search criteria.  I suggest adding the toLowerCase() method the end of elementValue on line 42.  Another drawback to this design is that the user does not know what options are available to them without glancing at the entire data list.  I suggest incorporating a drop-down list instead of a user input field so that the user can view all options. 
