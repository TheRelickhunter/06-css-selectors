##### 07-most-specific

Specificity in CSS rules declaration is like a measure that take in account how much selector, classes, IDs, pseudo-classes have been defined in a rule.
Next, a series of numbers separated by a comma are assigned for each rule, so that it is evaluated like priority levels.
Moreover these should be understood from left to right as follow:


 <sub>1</sub>x, <sub>2</sub>x,<sub>3</sub> x, <sub>4</sub> x 

1) css rule defined inline into the element (style attribute)
2) if there's IDs selectors defined on the rule these have the priority over classes/pseudoclasses and elements.
3) Classes,pseudoclasses,attributes selectors have the precedence over elements.
4) element selectors.

Just have in mind a few things:
- negation pseudoclass, relational selectors like descendant " ", Direct child selector ">", General sibling selector "~", Adjacent sibling selector "+" are discarded by the calculus.
- If there's two or more rule declaration with the same level of specificity then last one will be applied.

Some examples here:

```
ul li {}
```

level: 0,0,0,2

```
ul > li {}
```
level: 0,0,0,2
```
body > #main.mobile a:hover {}
```
level : 0,1,2,2
```
div p > span {}
```
level : 0,0,0,3
```
.users .name {}
```
level: 0,0,2,0
```
[href$='.pdf'] {}
```
level : 0,0,1,0
```
:hover {}
```
level : 0,0,1,0
```
div .name {}
```
level : 0,0,1,1
```
a[href$='.pdf'] {}
```
level : 0,0,1,0
```
.pictures img:hover {}
```
level : 0,0,2,1
```
.name.name.name {}
```
level : 0,0,3,0
```
.user #name {}
```
level : 0,1,1,0
```
#name span {}
```
level : 0,1,0,1

```
nav#nav > li:hover {}
```
level : 0,1,1,2
```
li:nth-child(2n+1):hover {}
```
level : 0,0,2,1