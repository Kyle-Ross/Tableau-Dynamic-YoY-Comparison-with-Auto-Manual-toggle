# Tableau Dynamic YoY Comparison
Tableau has the ability to change the month of financial year start built in. However, the selection you make is ignored within calculated fields. This becomes a problem when your client has a financial year that does not start in January, and you need to make complex customisations involving financial years and quarters. Most commonly this issue would arise when you want to create a DatePart selector.

With this modular solution you can easily overcome this limitation, with logic that accounts for all possible financial year starting months.
This will work with any date field, so just take the relevant calculated fields and parameters and drop them in your workbook. Then just set your desired financial year start month and you are good to go.

You can test this by swapping the Start Month Selector in the dashboard and watching the FY and Quarter values accurately update.
 
 ## Calculated Fields
- [Order Date (Year Offset)](https://github.com/Kyle-Ross/Tableau-Dynamic-FY-Start-with-datepart-toggle/blob/80f04ee26c14aa85dfb8c8efb59874f16f0e07db/Calculated%20Field%20Formulas/Order%20Date%20(Year%20Offset).txt) - Determines the correct FY for a given date based on the desired start month
- [Order Date (Quarter Offset)](https://github.com/Kyle-Ross/Tableau-Dynamic-FY-Start-with-datepart-toggle/blob/80f04ee26c14aa85dfb8c8efb59874f16f0e07db/Calculated%20Field%20Formulas/Order%20Date%20(Quarter%20Offset).txt) - Determines the correct quarter for a given date based on the desired start month
- [Date Part Option](https://github.com/Kyle-Ross/Tableau-Dynamic-FY-Start-with-datepart-toggle/blob/80f04ee26c14aa85dfb8c8efb59874f16f0e07db/Calculated%20Field%20Formulas/Date%20Part%20Option.txt) - Takes the other fields and creates the Date Part fields for use in your dashboards

 ## Parameters
- [Date Part Parameter](https://github.com/Kyle-Ross/Tableau-Dynamic-FY-Start-with-datepart-toggle/blob/80f04ee26c14aa85dfb8c8efb59874f16f0e07db/Calculated%20Field%20Formulas/Date%20Part%20Parameter.txt) - Selects the DatePart to show
- [FY Start Month Selector](https://github.com/Kyle-Ross/Tableau-Dynamic-FY-Start-with-datepart-toggle/blob/80f04ee26c14aa85dfb8c8efb59874f16f0e07db/Calculated%20Field%20Formulas/FY%20Start%20Month%20Selector.txt) - Sets the month in which the financial year starts
 
 ## Dashboard
   [![tableau dynamic FY Start](https://img.shields.io/badge/review_on_tableau_public-1DA1F2?style=for-the-badge&logo=tableau&logoColor=white)](https://public.tableau.com/app/profile/kyle.ross6552/viz/DynamicYoYComparison/DynamicYoYComparison)
 
 The view below is static. Click the link above to use and interact with the dashboard on Tableau Public.
 
<div class='tableauPlaceholder' id='viz1655720865475' style='position: relative'><noscript><a href='https:&#47;&#47;github.com&#47;Kyle-Ross&#47;Tableau-Dynamic-YoY-Comparison'><img alt='Dynamic YoY Comparison ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Dy&#47;DynamicYoYComparison&#47;DynamicYoYComparison&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='DynamicYoYComparison&#47;DynamicYoYComparison' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Dy&#47;DynamicYoYComparison&#47;DynamicYoYComparison&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-GB' /></object></div>
