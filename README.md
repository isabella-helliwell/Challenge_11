# Challenge_11
# 1.0 Project Overview
    The aim of this project is to create a filter for multiple criteria at the same time. The user can filter the table
    by either date, city, state, country, or shape.

# 2.0 Resources

   - Language: JavaScript, HTML
   - datasource: data.js

# 3.0 Coding Summary

    In html, the user is asked to enter date, city, state, country and shape. The user can enter either a single value input box
    or a multiple value input boxes. Each time the user presses enter, the data table is filtered in accordance with the user input criteria.
    
    In app.js, two functions are created, function updateFilters(), which will take the user input data from the html, and save the objects into
    a new object variable, filters{}.
    If a filter value is entered, it is added to the filters{}, list, if no filter value is added, the filter is deleted from the filters object.
    Next, a function is called to loop through the filters and keep any data that matches the filter value.
    The last step is to rebuild the table using the filtered data by calling the function buildTable().
    
    Also added, is an event to listen for changes to each input element and calls the updateFilters() function:d3.selectAll("input").on("change", updateFilters)
    
    
         
  
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

Filtering by country: Canada. The output is;
![image](https://user-images.githubusercontent.com/85843030/132239983-5419b10e-20d0-4edd-b638-558991dd62fd.png)

Finally what if we search for a criteria that does not exsist like date 9/6/2021, the output:
![image](https://user-images.githubusercontent.com/85843030/132240301-5acfa416-324b-44b2-98cc-61a35702b17b.png)



# 4.0 Summary
## 4.1 Additional improvements:

Although this webpage looks impressive, there is one clear drawback and that is the case sensivity of the input text. This can be fixed by converting
the input data to lowercase by adding "<input style="text-transform: lowercase;"/>" in the html code where the user input is.

![image](https://user-images.githubusercontent.com/85843030/132243903-36b54337-68e3-4017-947c-7b3039747024.png)

In this instance, the above line of code, stops the user inserting upper case to the "Enter a State" search.




## 4.1 Further development

It is difficult for the user to know what to filter on. Adding a scrollbar with the existing values to filter for is necessary.
After each search we also need to clear the filter so new filter searches can be entered.
