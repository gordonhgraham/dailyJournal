#8/9/16 Tuesday
##Intro to Cascading Stylesheets: CSS
####Anatomy of a Style
* Selector(p)  declaration--contains {property: value}
```p {color: red}``` --entire thing is called a rule
 
* Selector Types
	* Type selector
		* ```h1{ color:blue; }```
	* class selector
		* ```.menuItem{ width: 500px; }```

	* ID
		* ```#uniqueBox{ width: 500px; }```	

	* pseudo-selector
		* ```div:hover { color: pink; }```

####Specificity
* Specificity increases
	* Type --> Class --> ID --> Inline
* If specificity is equal, the last declaration win

####Inheritance in CSS
* Decendants inherit properties from parents
* If more than one selector is used to style an element, property styles from **both** selectors will style the element if no conflicts.

####Combinators
* Combine selectors with combinators to target very specific elements
	* decendant selector ``` ```(space) apples to all decendants
		* ```div p { color:blue; }```
	* child selector ```>``` applies to only child of parent element
		* ```div>p { color:blue; }```
	* adjacent sibling selector ```+```
		* ```#class+p { color:blue; }```
	* general sibling selector ```~```
		* ```#class~p { color:blue; }```

####Display
* Block, inline, inline-block, none
	* check [Learn article]() for default desplay value of common elements (ex: default for ```<div>``` is block)
	* [Default Inline]()
	* [Default Block]()

####Box Model
* [margin **border[**padding [Content] padding**]border** margin]
*  Box-Sizing:
	* ```box-sizing: content-box```**default**  when talking about width of box content-box refers to **content only**
	* ```box-sizing: border-box```when we change to border-box  we are talking about **content, padding, and border**