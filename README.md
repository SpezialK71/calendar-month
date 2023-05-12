# calendar-month
Calander Month Program.

The problem is to display a calendar month for any  
given month between January 1800 and December  
2099. The format of the month should be as shown:  

#### MAY 2012  
Sun Mon Tue Wed Thu Fri Sat  
------------1----2----3---4--5-  
-6----7----8----9---10--11--12  
13--14---15---16---17-18--19  
20--21---22---23---24-25--26  
27--28---29---30---31  


Need an algorithm for computing the first day of a  
given month for years 1800 through 2099...  

...and an algorithm for appropriately displaying  
the calendar month, given the day of the week that  
the first day falls on, and the number of days in  
the month.  


### DATA DESCRIPTION  
Year and month entered and stored as integer values.  
Represented by variables __year__ and __month__.  
  
             year = 2012    month = 5  
             
Remaining values will be computed by the program based  
on the given year and month, as given below,

    leap_year    num_days_in_month    day_of_week  

The variable __leap_year__ holds a Boolean (True/False) value.  
Variables __num_days_in_month__ and __day_of_week__ both hold  
integer values.  


### ALGORITHMIC APPROACH  

    a) determine day of week a given date falls on.
        1. Let *century_digits* be equal to the first two digits of the year.
        2. Let year_digits be equal to the last two digits of the year.
        3. Let __value__ be equal to __year_digits__ + floor(__year_digits__/4)
        
    b) determine how many days are in a given month.
    
