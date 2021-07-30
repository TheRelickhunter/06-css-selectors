# 04-we-mean-business

### Author details
##### #24 Andrea Zappa
***
<h4>Requirements</h4>

1. Create a table with details of business contacts
   - Columns can include : name , email address, country, etc (max 6 columns)
   - Fill the table with contents
2. Add a styles.css file. The HTML file should not contain any inline style!
3. The table header should have a background color
4. the table rows should have an alternating white/grey background 
   - Row 1 grey, row 2 white, row 3 grey etc
5. When the user hovers over a row with the mouse the color should change

<strong>Bonus</strong>: Modify your CSS so that the table row colors alternate every 2 rows.

<h4>My solutions</h4>

<!--
table thead {
    background-color: #DBC5FE;

}
table tbody tr:nth-child(odd) {
    background-color: grey;
}
table tbody tr:nth-child(even) {
    background-color: white;
}
table tbody tr:hover {
    background-color: #8EB2B2;
}
-->

3. Just use the descendant selector to refer to the ```thead``` element and apply the background color as required.
4. The use of ```:nth-child(odd)``` and ```:nth-child(even)``` position pseudoclasses selectors referring to the child ```tr``` of parent ```tbody``` match the requirements.
5. Same as point 4 we just pick the child ```tr``` of parent ```tbody``` but we use the ```:hover``` pseudoclass to define how styling the row when user hovers it.