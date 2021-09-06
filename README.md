# Challenge_11
# 1.0 Project Overview
    The aim of this project is to create a filter for multiple criteria at the same time. The user can filter the table
    by either date, city, state, country, or shape.

# 2.0 Resources

   - Language: JavaScript, HTML
   - datasource: data.js

# 3.0 Coding

    In html, the user is asked to enter date, city, state, country amd shape. The user can enter either a single value input box
    or a multiple value input box. Each time the user presses enter, the data table is filtered in accordance with the user input criteria.
    
    In app.js, two functions are created, function updateFilters(), which will take the user input data from the html, and save the objects into
    a new object variable, filters{}.
    If a filter value is entered, it is added to the filters{}, list, if no filter value is added, the filter is deleted from the filters object.
    
    
    Using Javascript, a function is created that saves the elements, value, and id of the filter that the user has set in the input
    boxes in the HTML code. 
    If a filter value is entered, than it will be added to the elementValue, otherwise the filter will be cleared from the filters object.
    The filter is applied to the table by using a function to filter the data.
    After looping through the filters, any data that macthes the filter values is kept. 
    For the final step, the table data is rebuild using the filtered data.
    
       
  
# 4.0 Results
  
  The webpage takes the user input and
  The webpage is user inetarctive and works using the user input parametres. For example, if we want to see all the UFO sightsings in california for
  date 1/4/2010, we get:
 ![image](https://user-images.githubusercontent.com/85843030/132144860-0dff7d3f-06d7-424a-aa0c-9669ccdc63cc.png)

If we want to filter further by shape, we can enter light and the outcome is:
![image](https://user-images.githubusercontent.com/85843030/132144902-dfdde1a5-c8a7-4315-98d6-847aa54bac4d.png)

Here we have filtered by date: 1/1/2010, state:fl, the output is:
![image](https://user-images.githubusercontent.com/85843030/132144969-cf72454e-4bd3-400b-af5d-5a1f39cfda41.png)

Here the filter is city: el cajon, and the output is:
![image](https://user-images.githubusercontent.com/85843030/132145013-e6b60631-8e39-48cc-a4de-1a4355347068.png)






  




  
  
  









# 4.0 Additional improvements:

The input deck is case sensitive, one way of fixing this, can be that we take the input and transform it to lowercase in the javascript
We could also add a count function to count how many sightings have been in countys. 
