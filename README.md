# Tableau Dynamic YoY Comparison with Auto/Manual toggle
A fully featured dynamic YoY Comparison dashboard, with automatic and manual date selection options.

In auto-mode, dates from the 'previous' year are automatically limited to those present in the data for the 'current' year. This automatically and easily prevents inaccurate YoY comparisons when viewing data for a year which is yet to be completed.

Manual mode allows the user to specify exactly the dates to be compared in the view.

This approach is modular and could be easily adapted to any combination of date field and metric.

The complex logic driving these features all occurs under the hood, with simple user customisable parameters allowing users to quickly and accurately perform YoY comparisons without any need for regular upkeep or maintence by the dashboard creator.
 
 ## Calculated Fields
- [DatePart (Year)](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/DatePart%20(Year).txt) - Gets the year of the date as an integer
- [Previous Year Sales](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Previous%20Year%20Sales.txt) - Only returns the sales for the selected 'previous' year
- [Current Year Sales](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Current%20Year%20Sales.txt) - Only returns the sales for the selected 'current' year
- [Previous Year Dates](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Previous%20Year%20Dates.txt) - Only returns the dates for the selected 'previous' year. Will automatically limit the dates of the 'previous' year to those which are available in the data for the 'current' year
- [Current Year Dates](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Current%20Year%20Dates.txt) - Only returns the dates for the selected 'current' year
- [Sales YoY Diff #](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Sales%20YoY%20Diff%20%23.txt) - Returns the # difference in sales between the 'current' and 'previous' sales
- [Profit YoY Diff %](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Profit%20YoY%20Diff%20%25.txt) - Returns the % difference in sales between the 'current' and 'previous' sales
- [Previous Year Dates (MIN)](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Previous%20Year%20Dates%20(MIN).txt) - At a fixed table scoped LOD, returns the minimum date from the 'Previous Year Dates' field
- [Previous Year Dates (MAX)](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Previous%20Year%20Dates%20(MAX).txt) - At a fixed table scoped LOD, returns the maximum date from the 'Previous Year Dates' field
- [Current Year Dates (MIN)](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Current%20Year%20Dates%20(MIN).txt) - At a fixed table scoped LOD, returns the minimum date from the 'Current Year Dates' field
- [Current Year Dates (MAX)](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Calculated%20Fields/Current%20Year%20Dates%20(MAX).txt) - At a fixed table scoped LOD, returns the maxium date from the 'Current Year Dates' field

 ## Parameters
- [Use Manual Dates Toggle](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison/blob/0d210dcdecc756673fa17d05385fbb99fc8d6494/Parameters/Use%20Manual%20Dates%20Toggle.txt) - Toggles between the functions which automatically select comparison dates vs those which allow you to manually set the dates.
- [Previous Year](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison-with-Auto-Manual-toggle/blob/9a15c6676d8c9f408b0c74eb4782ece537ca7ce1/Parameters/Previous%20Year.txt) - Defines the 'Previous' year as it is to be used in the calculations
- [Current Year](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison-with-Auto-Manual-toggle/blob/9a15c6676d8c9f408b0c74eb4782ece537ca7ce1/Parameters/Current%20Year.txt) - Defines the 'Current' year as it is to be used in the calculations
- [Previous Year Week Manual MIN](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison-with-Auto-Manual-toggle/blob/9a15c6676d8c9f408b0c74eb4782ece537ca7ce1/Parameters/Previous%20Year%20Week%20Manual%20MIN.txt) - Defines the bottom of the date range of the 'previous' year when using the manual option
- [Previous Year Week Manual MAX](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison-with-Auto-Manual-toggle/blob/9a15c6676d8c9f408b0c74eb4782ece537ca7ce1/Parameters/Previous%20Year%20Week%20Manual%20MAX.txt) - Defines the top of the date range of the 'previous' year when using the manual option
- [Current Year Week Manual MIN](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison-with-Auto-Manual-toggle/blob/9a15c6676d8c9f408b0c74eb4782ece537ca7ce1/Parameters/Current%20Year%20Week%20Manual%20MIN.txt) - Defines the bottom of the date range of the 'current' year when using the manual option
- [Current Year Week Manual MAX](https://github.com/Kyle-Ross/Tableau-Dynamic-YoY-Comparison-with-Auto-Manual-toggle/blob/9a15c6676d8c9f408b0c74eb4782ece537ca7ce1/Parameters/Current%20Year%20Week%20Manual%20MAX.txt) - Defines the top of the date range of the 'current' year when using the manual option
 
 ## Dashboard
   [![tableau dynamic FY Start](https://img.shields.io/badge/review_on_tableau_public-1DA1F2?style=for-the-badge&logo=tableau&logoColor=white)](https://public.tableau.com/app/profile/kyle.ross6552/viz/DynamicYoYComparison/DynamicYoYComparison)
 
 The view below is static. Click the link above to use and interact with the dashboard on Tableau Public.
 
<div class='tableauPlaceholder' id='viz1655720865475' style='position: relative'><noscript><a href='https:&#47;&#47;github.com&#47;Kyle-Ross&#47;Tableau-Dynamic-YoY-Comparison'><img alt='Dynamic YoY Comparison ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Dy&#47;DynamicYoYComparison&#47;DynamicYoYComparison&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='DynamicYoYComparison&#47;DynamicYoYComparison' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Dy&#47;DynamicYoYComparison&#47;DynamicYoYComparison&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-GB' /></object></div>
