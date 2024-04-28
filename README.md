
# Project Title


# Customer Analytics-Dashboard


## Problem Statement

This dashboard helps the companies understand their
customers better . It analyzes data and shows the customer count the organization has in the different market segments that it is operating in. It shows active customers over the years in the aforementioned segments. I t also uses a heat map to show the best performing or most selling products by the organization.

We can observe looking at the data that the segment with most active customers and in general the most customers is corporate sector. It also has the highest selling product (office machines)

### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : For calculating Customer per market segment, a new measure was created by applying the formula : 
Consumer Count = CALCULATE(DISTINCTCOUNT(Sheet1[Customer Name]),FILTER(Sheet1,Sheet1[Customer Segment] = "Consumer")) 
This process was repeated for all segments.
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Visual filters (Slicers) were added for four fields named  'Order Priority', 'Reigon','Ship Mode', & 'Product Category'.
- Step 8 : A bar chart was added to the report showing active customer count by each year. 
- Step 9 : A heat map was created by first inputting a matrix table of market segments and product sub category. After that through custom filtering I colored the highest values based on sales in comparison to the whole data. the darker values signify higher sales while the paler values signify low performing goods.

![image](https://github.com/FaizanHayatPannu/Power-Bi/assets/168118585/0c398f94-a175-49c7-b554-6c997717656c)
