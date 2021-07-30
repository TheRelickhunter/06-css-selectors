# 03-super-hot

### Author details
##### #24 Andrea Zappa
***
<h4>Requirements</h4>

The exercise require some modifications inside the CSS file to add some styles to the main html page.

1. Add a rule to make links and visited links dark orange
2. Add a rule that will make the table header have different background color.
3. Add a rule that will make the first cell in each data row have a red background and white text.
4. Add a rule that will "zebra stripe" the backgrounds of the rows, alternating between white and #eeeeee.
5. Add a rule that will turn the label red when the checkbox is clicked.
6. Add a rule that will make the first letter of the pepper name huge and bold.
7. Add a rule that will find any pepper that is superhot and color the link red.

<h4>My solutions</h4>

1. In order to be effective we use ```a:link``` and ```a:visited``` pseudoclasses to apply the property ```color``` directly to the text content inside every anchor element.
2. Using the selector ```tr th``` descendant selector we make a change to the background color to the table header ```th``` that is within the ancestor element ```tr``` .
3. The pseudoclass selector ```:nth-child(n)``` is useful in that case because will select each ```td``` element which contain the content of the table that is interpreted as child element to the ```tr``` row element.
4. The pseudoclass selector ```:nth-child(2n)``` will style every even row table ```tr``` with the background color white and the ```:nth-child(2n+1)``` applied to every odd row the light-grey color.
5. Selecting with the selector ```input[type=checkbox]:checked ~ label``` we combine the next sibling element selector to the state pseudoclass ```:checked``` over the attribute selector to the input element to say "when checkbox checked apply the style properties to the label".
6. Using the ```td:nth-child(2):first-letter``` textual pseudoelement selector with structure selector ```:nth-child()``` pick the first character letter in the text content and apply some style properties upon the ```td``` element.
7. the ```td a[title*="superhot"]``` will select each anchor element with attribute ```title``` that contain the exact word "superhot" using the ```*=``` operator.