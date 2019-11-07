## Introduction
Selectors are the way we identify User Interface elements on the screen. They are a xml string which contain some properties that uniquely 
define the specified element. 

A selector has the following structure: ```<node_1/><node_2/>...<node_N/>```

Each node has the following format:  ```<ui_system attr_name_1='attr_value_1' ... attr_name_N='attr_value_N'/>```

* A selector contains 2 types of information: the element type and one or more of its attributes.
* Selectors should be constructed in such a way that they point to only one element
in the environment. If a robot finds multiple possible matches for a selector, it uses the first one it encounters – usually the topmost one
* When automatically building a selector, UiPath tries to use only the first and last
container but it also adds intermediate ones only needed

## Types of Selectors
### Full Selectors: 
Contains all the elemts needed to locate a UI element including top level window
### Partial Selectors: 
Does not include top elements, used to prevent interference from other instances of the window/application.

*Basic recording generates full selectors while Desktop recording generates only partial ones.*

## Building our own Selector

* We can build dynamic selectors using the 2 available wildcards: question mark (?) takes the place of a single character and asterisk (*) that replaces any
number of characters or by using variables.
* Use Attach to live element to update an existing selector to also match a 2nd element.
* Use the selector’s idx property to get a certain occurrence of an element that is found multiple times.
* Use idx attribute as last resort if idx value is greater than 2.
* Add other attributes to make sure the selector is stable.

## Debugging Selectors
Use the Validate and Repair option in UI Explorer or Select Editor window.

## Alternative to Selectors
These alternatives can be used to build reliable automation when the selectors are not very stable. 
1. Anchor Base activity:
It uses the position of elements on screen and doesnot work in background.
2. Select Relative Element in UiEplorer
It is dependent on the internal structure of the application
and works in background as well.

