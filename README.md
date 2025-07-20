# tables
Repository for tables
## Accessibility in tables
* Proper markup helps screen readers deliver content appropriately to visually impaired users who use screen readers to access websites.
* Using markup that include columns and row headers allows us to replace visual associations between table columns and rows with programmatic associations. 
## Core Elements of Table Accessibility
1. Using columns and rows headers: Combination of column and row headers faciliates interpretation of table data based on the relationship exisiting between headers and tables they represent. 
2. Using `caption` to add captions to the table: This is done by nesting a `caption`element below the opening `table` tag.
3. Adding structure with `thead`, `tbody`, and `tfoot`: facilitates one to make a header, body, and footer section for a table. The elements don't add any visual enhancement to the table or increase their accessibility but they are beneficial for applying styling and layout enhancements with CSS. 
`thead`: Must wrap the part of the table that is the header - typically the first row containing the column headngs.
`tbody`: Wraps the main part of the table content that isn't the table header or footer. 
`tfoot`: wraps the part of the table that is the footer. Could be the final row with items in the previous row summed up. 
4. The `scope` attribute: The attribute can be used to tell the screen readers exactly what cells the header is a header for. 
5. `id` and `headers` attribute: Alternative to the `scope` attribute. Used to create associations between data cells and header cells. 
 A `th` element can provide a heading for either a data cell (`td`) or in more complex tables, for another header cell (`th`). This facilitates creation of layered or grouped headers where one header describes several others. 
 The `headers` attribute is used to link a cell, `td` or `th`to one or more header cells. 
