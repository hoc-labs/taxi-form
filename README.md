# Advanced Form Styling

In this lab you're going to build a form to schedule a pick-up from a taxi company.

We'll use both grid and flex to layout the form. The HTML structure will be supplied, but you need to build the CSS for the layout as well as the form element styles.

## Grid Areas
An easy way to specify the grid structure is to use the grid-template-areas property on the grid container element. All you have to do is create the rows using strings representing the columns each area takes up in each row.

In this form the top row will have two columns and the bottom row will have one column, so we just duplicate the bottom area for both columns. Then we define a style that is associated with the grid area.


![](https://raw.githubusercontent.com/hoc-labs/images/main/taxi-form-1.png)

## Left Region Flex
Each label/input pair is grouped in a `<div>` with the class of "input-group". These will flow from top to bottom on their own. On the input-group `<div>`, we set the display property to flex to get each child `<label>` and `<input>` element pair to flow from left to right.

## Right Region Flex
Each `<fieldset>` element will flow from top to bottom on their own. On the `<fieldset>`, we set the display property to flex to get the fieldset child elements to flow from top to bottom.

![](https://raw.githubusercontent.com/hoc-labs/images/main/taxi-form-2.png)

## Flex-grow
The flex-grow property specifies what happens to the element when distributing extra space across the width of the container. The default value is zero. Set the value to one for the form elements to the right of the labels, so that they will stretch to fill the available space and the label will remain a fixed size.








