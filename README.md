# SQL-TaskEduBridge
Step 1: Enter the values to the excel as table formate and save it.

Step 2: In the Cell below the Duplicate Name column just do the Logic to populate the duplicate name field for names that occurs more than once

   =IFERROR(INDEX([[Customer name ]],MATCH(0,COUNTIF(B1:$B$1,[[Customer name ]])+IF(COUNTIF([[Customer name ]],[[Customer name ]])>1,0,1),0)), "")
In this Logic the [[[Customer name]] is the selected value cell from the excel. Actually that is (A2:A17)

If your Excel also updated then it will display us like the column header name
