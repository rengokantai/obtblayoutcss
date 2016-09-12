### obtblayoutcss
####Chapter 1. Table Layout in CSS
#####Table Formatting
######Visually Arranging a Table
CSS draws a distinction between table elements and internal table elements.  
In CSS, internal table elements generate rectangular boxes that have content, padding, and borders, ```but not margins```.  

Table arrangement rules
-  


######Table Display Values
table:table  
table-row:tr  
table-row-group:tbody  
table-header-group:thead  
table-footer-group:tfoot  
table-column:col  
table-cell:td
table-caption:?  

specification:
```
table {display: table;}
tr {display: table-row;}
thead {display: table-header-group;}
tbody {display: table-row-group;}
tfoot {display: table-footer-group;}
col {display: table-column;}
colgroup {display: table-column-group;}
td, th {display: table-cell;}
caption {display: table-caption;}
```


Row primacy:  
CSS defines its table model as “row primacy.”  
In other words, the model assumes that authors will create markup languages where rows are explicitly declared.  

######Anonymous Table Objects
This table needs a tr element.
```
<table>
  <!--anonymous table-row object begins-->
    <td>Name:</td>
  <!--anonymous table-row object ends-->
</table>
```
If a table-cell element’s parent is not a table-row element(i.e.table or table-row-group), then an anonymous table-row object is inserted between the table-cell element and its parent.  

