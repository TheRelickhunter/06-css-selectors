# 05-chessboard

### Author details
##### #24 Andrea Zappa
***
<h4>Requirements</h4>

1. Create a table with 8 rows and 8 columns.
2. Your ```<td>``` elements should be empty (or contain one letter when nedeed).
3. Use CSS selectors to crate a chessboard pattern like int the image below.
4. You may use the following rule to fill the table cells.

<h4>My solutions</h4>

<!-- 
td {
    height: 20px;
    width: 20px;
}
tr:nth-child(odd) td:nth-child(1n) {
    background-color: orange;
    }
tr:nth-child(even) td:nth-child(1n) {
    background-color: black;
}
tr:nth-child(1n+1) td:nth-child(2n) {
    background-color: black;
    }
tr:nth-child(2n) td:nth-child(2n) {
    background-color: orange;
}

-->

1. A shortcut to create many rows and columns would be using the Emmet plugin so just by typing 
  ```table > tbody >tr * 8``` and ```td * 8``` by placing the cursor inside the ```tr``` element we create the table in a snap.
3. To reproduce the pattern as shown I picked with the first two rules the vertical pattern by using ```tr:nth-child(odd) td:nth-child(1n)``` and ```tr:nth-child(even) td:nth-child(1n)``` .
   The second pattern is horizontal with the last two ones ```tr:nth-child(1n+1) td:nth-child(2n)```
   and ```tr:nth-child(2n) td:nth-child(2n)``` .
   

<h5>Notes:</h5>
Emmet plugin is extremely useful when you have to build structured snippets of HTML code in development stage. It's simple to use because it is based on CSS constructors so just by typing you get the results and avoid long times of typing repetitive code.