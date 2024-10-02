# blinkit-India's Largest Grocery App 

### Dashboard Link : https://drive.google.com/file/d/11W3Ncr4eyVB2KlUOrhUsF5EIyctIWK8Q/view?usp=drive_link

## Problem Statement

This dashboard helps the blinkit understand their customers better. It helps the blinkit know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average Sales, thus since by using this dashboard they have identified this problem, they can further work on factors responsible for further improvement of sales.

blinkit further understand their sales based on Outlet Size,Location Type and Item type (Which Products customer liked most -- We can filter this for various location ,year or month)


### Steps followed 

- Step 1 : Business Requirement
- Step 2 : Data Walkthrough
- Step 3 : Data Connection
- Step 4 : Data Cleaning/Quality Check
- Step 5 : Data Modelling
- Step 6 : Data Processing
- Step 7 : DAX Calculations
- Step 8 : Dashboard Layouting
- Step 9 : Charts Development and Formatting
- Step 10 : Dashboard/Report Development

  (a) Total Sales

  (b) Average Sales
  
  (c) Number of Items
  
  (d) Average Rating
  
  (e) Sales Analysis based on Outlet Establishment
  
  (f) Sales Analysis based on Fat Content

  (g) Sales Analysis based on Outlet Size and Type
  
  
In our dataset, Some parameters were assigned value 0, representing those parameters are not applicable for some customers.

All these values have been ignored while calculating average rating for each of the parameters mentioned above.

        
 - Step 11 : New measure was created to find Total Sales,Average Sales,Total Items and Average Rating
 
 Following DAX expression was written to find above mentioned parameters
 
 Total Sales = SUM('BlinkIT Grocery Data'[Sales])

 Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

 No Of Items = COUNTROWS('BlinkIT Grocery Data')

 Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

 Metrics = {
    ("Total Sales", NAMEOF('BlinkIT Grocery Data'[Total Sales]), 0),
    ("Avg Sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1),
    ("No Of Items", NAMEOF('BlinkIT Grocery Data'[No Of Items]), 2),
    ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 3)
}


 
 # Report Snapshot (Power BI DESKTOP)

 
![Screenshot (9)](https://github.com/user-attachments/assets/38e4cfdf-baa3-41e8-91e1-fff54bc2af6a)

# blinkit Dashboard

![blinkit Dashboard](https://github.com/user-attachments/assets/cbec22f8-dae4-4d77-ad5b-91cde4f75977)



# Insights

A single page report was created on Power BI Desktop

Following inferences can be drawn from the dashboard;

### [1] Total Number of Sales = $ 1.20 M 
###     Average Sales = $ 141 M
###     Total Number of Products Available = 8523
###     Average Rating = 3.9

![Sales Card](https://github.com/user-attachments/assets/7209f595-c9ce-4e7a-bcee-2b1a4e060d5e)
           
### [2] Fat Content

Low Fat Content are sold more than Regular,Fruits and Veggies Hold the Big Sales compared to others

    a) Low Fat Sales  - $ 425.36k
    b) Regular Sales - $ 776.32k
    c) Tier 3 outlet Total sales is higher among tier 2 and tier 3 outlet
    d) Snacks ,Fruits and Veggies total sales - $ 0.18M

![Fat Content](https://github.com/user-attachments/assets/c85e7cc3-3abd-4c7c-bb07-462fe0176c81)
  
  while calculating average rating, null values have been ignored as they were not relevant for some customers. 
  
  These ratings will change if different visual filters will be applied.  
  
  ### [3] Outet Establishment 
  
      Outlet Established in 2018 Got more sales - $205k

![out est](https://github.com/user-attachments/assets/b3eb033a-0225-418c-8f6b-7ce5492a0423)


 ### [4] Some other insights
 
 ### Class
 
 1.1) Medium Size Outlets Sold more items.
 
 1.2) Supermarket Type 1 is mostly used by customer to purchase
 
 1.3) Tier 3 Cities outlet sales is high as compare to tier 1 and 2

![out Type](https://github.com/user-attachments/assets/30e4e3de-0fbe-45ce-953b-687295433048)

 
        
