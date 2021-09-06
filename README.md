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
    Finally some background images and some coloring has been added to the html code to make the page unique.
    
         
  
# 4.0 Results
  
  ![image](https://user-images.githubusercontent.com/85843030/132246335-d931cb32-48ea-4fa5-8bfa-4f3358177d4b.png)

  
  The webpage is user inetarctive and works using the user input parametres. For example, if we want to see all the UFO sightsings in california for
  date 1/4/2010, we get:
 ![image](https://user-images.githubusercontent.com/85843030/132246485-96f03c34-e3f8-4730-a9f9-aab5464bce67.png)

If we want to filter further by shape, we can enter light and the outcome is:
![image](https://user-images.githubusercontent.com/85843030/132246615-bfdccd53-9107-423a-b291-c95afcede6ef.png)


Here we have filtered by date: 1/1/2010, state:fl, the output is:
![image](https://user-images.githubusercontent.com/85843030/132246695-4930ecb5-058d-4558-a828-5d6611e7c0be.png)


Here the filter is city: el cajon, and the output is:
![image](https://user-images.githubusercontent.com/85843030/132246802-c825d6c1-55a8-4689-ba7a-1fb1d8a7258f.png)


Filtering by country: Canada. The output is;
![image](https://user-images.githubusercontent.com/85843030/132246863-2f960902-862b-4c96-a293-17fc5802bf2f.png)



Finally what if we search for a criteria that does not exsist like date 9/6/2021, the output:
![image](https://user-images.githubusercontent.com/85843030/132246934-cd86a64a-b052-4ad6-97f8-e12bf6263aee.png)




# 4.0 Summary
## 4.1 Additional improvements:

Although this webpage looks impressive, there is one clear drawback and that is the case sensivity of the input text. This can be fixed by converting
the input data to lowercase.

## 4.1 Further development

It is difficult for the user to know what to filter on. Adding a dropdown list with the existing values to filter for is necessary.
After each search we also need to clear the filter so new filter searches can be entered.
