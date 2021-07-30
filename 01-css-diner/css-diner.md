### 01-css-diner-game

## solutions

#### level 1
I've to select all elements of type A that means anchors, just to type the element type, but in this case we gonna select all the elements of type ```plate```.
```
plate {

}
```
---
#### level 2 

Same as level 1 but just select the ```bento``` element.

#### level 3 
Select the elements containing a certain ID i'm using the rule ```#fancy``` which use the ```#``` to select the id attribute.

----
#### level 4 
Select the elements inside another element identified as the ancestor by using the space.
The apple element bouncing can be selected with ```plate apple``` .
#### level 5
Select the element bouncing on the plate by using ```#fancy pickle``` .
In this case can be used by combining the ID selector ```#fancy``` and the element inside ```pickle```.

#### level 6
As the level 3 I should select elements even with the class selector.
Selecting the apples bouncing by using ```.small```.
#### level 7
Select elements with element dot class selector combined referring to all ```orange``` elements containing also class ```small```.

Picking them with ```orange.small``` .
#### level 8
This level would summarize all the ways to select elements learned previously. To solve this just select ```bento orange.small``` .
#### level 9
select the elements by using the comma operator is another way to select multiple elements by not taking in account the access level inheritance.
Typing ```plate, bento``` will pick these bouncing elements.

#### level 10
Select all the elements by using the operator ```*``` to satisfy the objective, everything on the table should be styled.
#### level 11
Only the objects onto the plate should be assigned with a style by ```plate *``` selector which select all elements inside the ancestor element ```plate```.
#### level 12
To select only the apples next the plates we use the adjacent sibling selector ```+``` referencing the ```<apple \>``` element that is sibling to ```<plate \>``` , so to solve this we must type ```plate + apple```.

#### level 13
Picking all the elements of the same type that are sibling of a specific elements we use ```~``` .
To pick the green pickles next to the bento we type ```bento + pickle``` .

#### level 14

I'm using the descendant element selector ```>``` to refer the apple nested into the plate.
```plate > apple``` will do that.
#### level 15
to select a first child element inside of another element, use the ```:first-child``` pseudo selector.
To solve this level we select first orange by typing ```orange:first-child``` .

#### level 16
To select an elements that is the only child element i'm using the Only Child pseudo selector ```:only-child``` .
So to reference the content onto the plate (apple,pickle) use  ```plate apple:only-child, plate pickle:only-child```.
#### level 17
You can use this selector to select an element that is the last child element inside of another element.
We use ```plate apple:last-child, pickle:last-child``` to select the last element (apple) onto plate, and last pickle onto the table.
#### level 18
Selects the nth child element in another element. To solve this, use ```plate:nth-child(3)```
#### level 19
bento:nth-last-child
```:nth-last-child(n)```
Select an element by its order in another element, counting from the back.
Use the ```bento:nth-last-child(3)``` to get the bento bouncing as it is the third element starting from the last bento.
#### level 20
Select the first element of a specific type.
Solving this we have to get the first element of type apple.

```
apple:first-of-type
```
#### level 21
Selects a specific element based on its type and order in another element - or even or odd instances of that element.

The second, forth, and sixth element of type plate selected by the ```plate:nth-of-type(even)``` .

#### level 22
The nth-of-type formula selects every nth element, starting the count at a specific instance of that element.

to select the plates every three steps with a gap of 2 we use that pseudo selector.
```plate:nth-of-type(2n+3)```

#### level 23
Select elements that are the only ones of their type within their parent element

Selecting the only apple onto the plate we use
```plate apple:only-of-type```

#### level 24

Select the last element of a specific type. We gonna use 

```orange:last-of-type,apple:last-of-type``` to pick the last orange element and last apple element.

#### level 25
Selects elements that don't have any other elements inside of them.

In order to solve this level we use pseudo selector 
```bento:empty```
to just select the bento elements with no elements within.

#### level 26
??? TBD
#### level 27
Select all elements that have a specific attribute.
To get the elements bouncing with labels the attribute selectors
``` plate[for],bento[for],apple[for]```
must be used combining the multiple type selector ```, ```.

#### level 28
Same as level 27 but we want to select only the elements of type plate with attribute for.

```plate[for]```

#### level 29
Select all elements that have a specific attribute value.
type the ```bento[for="Vitaly"] ```
to only select that elements which have attribute for and value Vitaly.
#### level 30
Select all elements with an attribute value that starts with specific characters.
Solution is by using the attribute selector and the ```^``` before the equal sign.
So ```*[for^="S"]``` .

#### level 31
Select all elements with an attribute value that ends with specific characters.
Solving this level with the attribute selector and the ```$ ``` to refer any element with an attribute value ends with "ato".
```*[for $="ato"] ```

#### level 32
Select all elements with an attribute value that contains specific characters anywhere.

If I want to select elements with an attribute value that contains values matching a series of characters I use the attribute selector with ```*``` before the equal sign.

```bento[for *="obb"] ```