# SNOW-CSS

- CSS stands for Cascading Style Sheets 
- It is a language for styling HTML documents by specifying certain rules for layout and display in key/value pairs. 
- Style Sheets are a simple and powerful method of allowing attachment of rendering information to HTML documents. 
- It used to style the webpages by setting background-color, font color, font size, font family, etc.
- A CSS consists of a set of rules that defines the styles for a web page. 
- A CSS style rule composed of selectors and declarations. 
- The selector is an HTML Element like h3 used in the below example. 
- The declaration is comprised of a property and a value surrounded by curly braces. 
- In the below example font-family, font-style and color were properties of the selector h3. Arial, italic and red were the values assigned, respectively, to the properties.
![image](https://user-images.githubusercontent.com/12488769/148694866-88327dcb-6106-4b02-93b4-4899a8e285ea.png)

## CSS Box Model
- The CSS box model used to determine how our web page is rendered by browser. 
- It considers each element on the page as a box, CSS allows you to apply different properties that define where and how that element appears. 
- Web pages are made up of rectangular boxes arranged and related to each other.
- Every box has 4 parts - margin, border, padding and content. 
- The margin is an outermost box, inside that the border, then padding, then the content is innermost. 
- All box sizes/formatting can be styled with CSS.
![image](https://user-images.githubusercontent.com/12488769/148694913-5bd75c48-81cc-4603-b6a4-dcd2d957b27c.png)
- Margin - It is a space between border and margin. It is useful to separate the element from its neighbors. The dimensions are given by the margin-box width and the margin-box height.
- Border - It is the area between the box’s padding and margin. Its dimensions are given by the width and height of the border.
- Padding - It is a space around the content area and within the border-box. Its dimensions are given by the width of the padding-box and the height of the padding-box.
- Content - It consists of content like text, image, or other media content. It is bounded by the content edge and its dimensions are given by content-box width and height

## Types of CSS
There are three types of CSS which are given below:
- Inline CSS
- Internal or Embedded CSS
- External CSS

## Inline CSS 
Inline CSS contains the CSS property in the body section attached with element is known as inline CSS. 
This kind of style is specified within an HTML tag using style attribute
![image](https://user-images.githubusercontent.com/12488769/148694963-15ce5402-d3de-4a86-94c0-1b39418667fb.png)

## Internal or embedded CSS
This can be used when a single HTML document must be styled uniquely. 
The CSS rule set should be within the HTML file in the head section i.e the CSS is embedded within the HTML file.
![image](https://user-images.githubusercontent.com/12488769/148694993-44a04abe-0f70-400c-b064-b405d87eeb84.png)

![image](https://user-images.githubusercontent.com/12488769/148694996-ad2c83cb-aa5c-45ad-9232-d9abc3e50d90.png)

## External CSS
- External CSS contains separate CSS file which contains only style property with the help of tag attributes.
- CSS property written in a separate file with .css extension and should be linked to the HTML document using link tag. 
- This means that for each element, style can be set only once and that will be applied across web pages.
![image](https://user-images.githubusercontent.com/12488769/148695017-12231141-1339-4877-bda8-3b0b75d51500.png)
```
- We have HTML file that makes use of the above created external style sheet (style.css). 
- This can be achieved by using <link> tag. 
- The <link> element has rel and href attributes. 
- The rel specifices the relationship between the current document and the linked document. 
- In this case, rel attribute value will be stylesheet because we going to add the external style sheet to the HTML document. 
- The href attribute is used to specify the location of the external style sheet file.
```

![image](https://user-images.githubusercontent.com/12488769/148695063-a455fcc6-3c8b-48a8-9a47-e359c0069f09.png)
![image](https://user-images.githubusercontent.com/12488769/148695067-5713265b-00fa-44c7-84d9-a589552b34c2.png)

## CSS Properties
- There are a number of CSS properties that you can use to style our webpage. 
- Here we'll discuss some of the CSS properties such as Border, Padding, Margin, display, position, color,and text-align.

## CSS Border Property
- The CSS border property allows to style the border area of a box.
![image](https://user-images.githubusercontent.com/12488769/148695118-cce6da03-f1d4-4aad-a676-9c8f859dddcc.png)

## CSS Padding Property
- The CSS padding property allow you to set the padding area for an element that separates its border from its content. 
- The padding property can take one, two, three, or four values separated by white spaces as listed in the below table. 
- Depending on the list of property values, the HTML element has the padding area on the top, bottom, right, and left.
= The padding property is a shorthand property for the padding-top, padding-right, padding-bottom, and padding-left properties

![image](https://user-images.githubusercontent.com/12488769/148695145-bcbfad5e-a835-48bb-8d0a-b69ad41fe1cb.png)

![image](https://user-images.githubusercontent.com/12488769/148695154-db31a16c-0f76-437d-bd94-47bb0ebcc90e.png)

## CSS Margin Property
- The CSS margin property is similar to the CSS border property, but it sets the margins around the sides of an element's box instead of the border. 
- It also takes one, two, three, or four values separated by white spaces. 
- The shorthand properties are margin-top, margin-right, margin-bottom, and margin-left to set a margin on respective sides.
![image](https://user-images.githubusercontent.com/12488769/148695179-61ce2fc0-b320-4beb-ae27-f6c81217df77.png)

## CSS Display property
- The display property controls the display behavior of an element. 
- The CSS display property sets whether an element is treated as a block or inline elements and the layout used for its children, such as flow layout, flex or grid.
- The Syntax for the display property is selector {display: value}
behaves likes block-level elements
![image](https://user-images.githubusercontent.com/12488769/148695206-8637306d-7f42-4274-ac27-4a00bf7c7d40.png)

## CSS Position Property
- The position property defines how an element will be arranged on a page. 
- The Syntax for the position property is selector {position: value}. 
- The property values are 
Static
Relative
Absolute
Fixed
inherit.

- static - The element's box is arranged automatically consistent with the normal flow.
- relative - The element's box position is relative to its normal flow position. You can adjust the normal flow position by using the top, bottom, left and right properties.
- absolute - The element's box arranged to an absolute position with reference to its containing block. Its containing block is that the nearest ancestor element that has its position property set to relative, absolute, or fixed. The top, right, bottom, and left properties are used to set the offset of the element's box with reference to its containing block.
- fixed - The element's box position is offset from its browser window by using the top, right, bottom, and left properties. The element's box won't move when the browser window is scrolled.
- inherit - The inherit keyword is employed to specify that the value for this property should be taken from the parent element. If inherit is used with the root element, then the initial value for this property is going to be used.
![image](https://user-images.githubusercontent.com/12488769/148695247-ad9ce405-72f8-4904-a8ae-d98822228da2.png)
## CSS Color property
The color property is used to specify the foreground color of text.
The color properties are set using 5 different color notation types 
![image](https://user-images.githubusercontent.com/12488769/148695265-77cce272-d216-4ee4-8b38-ed1603c2327c.png)

## CSS text-align property
- The text-align property is used to align the content inside the element. 
- The text inside the element can be aligned in 4 ways - left, right, center and justify.
![image](https://user-images.githubusercontent.com/12488769/148695290-13fcd6b2-11d6-4f65-b4b6-acb48d993282.png)


# CSS Selectors
- CSS selectors are used for selecting the content/text you want to style in our site. 
- Selectors are the part of CSS ruleset. 
- CSS selectors select the HTML elements according to its id, class, type, attribute, etc. 

## There are several different types of selectors in CSS, some of them are listed below
- Element Selector 
- Id Selector 
- Class Selector 
- Universal Selector 
- Attribute selectors 
- Grouping Selector 
- Child and descendent selectors 
- General and adjacent sibling selectors 
= Pseudo-element and pseudo-class selectors

## Element selector
The element selector selects HTML elements by their name / tag name like a, h1, div, p etc
![image](https://user-images.githubusercontent.com/12488769/148695626-759fa3da-c2ca-4af0-b0e9-5401c2fa6d5d.png)

## ID Selector
- In the CSS, the ID selector is a name preceded by a hash character (“#”). 
- It uses the id attribute of an HTML element to match the specific HTML element. 
- The id of an element should be unique within a page, so the id selector is used to select one unique element.


![image](https://user-images.githubusercontent.com/12488769/148695654-2d09bf9b-db20-4976-8b58-d0dc6d7c83a8.png)
![image](https://user-images.githubusercontent.com/12488769/148695656-c8caaabc-d48f-4823-88e2-6b7afcfa6f39.png)

## Class Selector
- In the CSS, the class selector is a name preceded by a period (“.”). 
- It uses the class attribute of an HTML element to match the specific HTML element. 
- We can have a Class selector specific to an HTML element like we have p.class in the below example.

![image](https://user-images.githubusercontent.com/12488769/148695688-d9a633f9-4033-425a-86bc-e658811f2b2c.png)

![image](https://user-images.githubusercontent.com/12488769/148695695-a75ac0b3-f024-471a-b2d9-fdc43932582a.png)

## Universal Selector
- The universal selector denoted by an asterisk (*), matches all the elements on the page. 
If any other specific selector exists on the element, then the universal selector will be omitted.

![image](https://user-images.githubusercontent.com/12488769/148695739-84a785f6-a093-424a-8cc3-c9aef13d27cf.png)

![image](https://user-images.githubusercontent.com/12488769/148695744-448a460d-07ca-47e2-bc9a-2196c12fac3b.png)

## Attribute Selector
```
An attribute selector selects the HTML elements that has a specific attribute or attribute with a specified value. 
You can create an attribute selector by having the attribute in a pair of square brackets [attribute]. 
The most commonly used attribute selectors are listed below:
[attribute] Selector - applies the style rule for all the element which has a specified attribute.
[attribute="value"] Selector - uses the = operator to select the element whose attribute value is exactly equal to the given value.
[attribute~="value"] Selector - uses the ~= operator to select elements that have the specified attribute with a value containing a given word, delimited by spaces.
[attribute|="value"] Selector - uses the |= operator to select elements that have the specified attribute with a value either equal to a given string or starting with that string followed by a hyphen (-).
[attribute^="value"] Selector - uses the ^= operator to select elements that have the specified attribute with a value beginning exactly with a given string.
[attribute$="value"] Selector uses the $= operator to select elements that have the specified attribute with a value ending exactly with a given string. The comparison is case sensitive.
[attribute*="value"] Selector - uses the *= operator to select elements that have the specified attribute with a value containing a given substring.
![image](https://user-images.githubusercontent.com/12488769/148695870-52457b19-cc57-4e11-b714-3134e17b38d9.png)

```
![image](https://user-images.githubusercontent.com/12488769/148695879-beb2c3c4-e311-4d5d-8204-886cd6a06a3a.png)
![image](https://user-images.githubusercontent.com/12488769/148695885-6f349480-3e8a-4917-85c6-f1869307a737.png)

## Grouping Selector
The CSS grouping selector is used to apply a common style for the number of elements on the page. 
You can group the selector using comma (,) separator. 
It allows you to specify the same properties and rules for more than one element at the same time. 
This reduces the code and extra effort to declare common styles for each element.
![image](https://user-images.githubusercontent.com/12488769/148695911-a4979871-df9f-45b7-87ad-6885606e89de.png)
![image](https://user-images.githubusercontent.com/12488769/148695921-a9223217-50a0-4dd4-86c2-d27ef241b3ed.png)

## Child Selectors
Child Selector selects all the elements that are the children of a specified element. 
The Syntax of Child Selector is element > element { property: value;} which selects those elements which are the children of specific parent. 
The left side of > is a parent element and on the right is the children element.

![image](https://user-images.githubusercontent.com/12488769/148695940-3afdba49-7537-4080-9dcf-781717ac450c.png)
![image](https://user-images.githubusercontent.com/12488769/148695946-fdaea086-1acd-4995-b5e1-51cd86af8df3.png)

## Descebdebt selectors
The descendant selector selects all the elements which are a child of the element. 
It allows you to limit the targeted elements to the ones who are descendants of another element. 
The syntax is element element { property: value; } you simply write the parent(s), separate with space, and then the actual element you want to target.

![image](https://user-images.githubusercontent.com/12488769/148695992-bc96c7fb-a48e-4b73-ab21-aa15ae9eeaf7.png)
![image](https://user-images.githubusercontent.com/12488769/148695998-fa85f7f0-2ed4-4d8c-b375-ed1860f2aeb6.png)

## General sibling selector
The General Sibling selector selects all the elements which are siblings of a specified element. 
The syntax is element ~ element { property: value; }, which selects all the sibling elements that are in same hierarchy level

![image](https://user-images.githubusercontent.com/12488769/148696028-5ef4f30c-f3f0-4863-bfa7-8c37cfb7f06f.png)
![image](https://user-images.githubusercontent.com/12488769/148696036-e77c6d7b-3c8f-4abd-b9b9-c5850a43ec43.png)

## Adjacent Sibling Selector
The Adjacent Sibling selector selects the element that are the adjacent sibling of a specified element. 
The syntax is element + element { property: value; }, which selects the second one, if it immediately follows the first one in order of appearance in an HTML page.
![image](https://user-images.githubusercontent.com/12488769/148696078-dadf0c23-79be-45d2-baa6-e1e6a42360f1.png)
![image](https://user-images.githubusercontent.com/12488769/148696084-1bd7334c-d44b-46a3-968e-d105bd4c462f.png)

## Pseudo Class Selector
```
Pseudo Class Selector is used to specify the state of an element. 
It let us to apply a style to an element which are related with external factors like the history of the navigator ( like :visited), the status of its content (like :checked on certain form elements), or the position of the mouse (like :hover, which lets you know if the mouse is over an element or not).
The syntax for Pseudo Class Selector is selector:pseudo-class { property: value; } . 
These pseudo- classes are used with the selector to style the element on a specific state.
:link - Used to select only <a> element with href attributes and applies the style for unvisted link. 
:visited - Used to select only <a> element with href attributes and applies the style for visited link. 
:active - selects an element which is activated by user clicks 
:hover - selects the style when the element is in its hover state (mouse cursor rolls over the element). 
:focus - selects the form input element that has received focus. It is generally triggered when the user clicks or taps on an element or selects it with the keyboard's "tab" key. 
:lang - Used to specify a language to use in a element. 
:first-child - selects the first element among a group of sibling elements
  ```
  ![image](https://user-images.githubusercontent.com/12488769/148696117-989eb501-1478-4841-a4c4-d2c8dc4c8cd8.png)

  ## Pseudo element  selector
  Pseudo-elements allows to style the specified parts of an element that is not available under DOM tree. 
It let us to apply to style the first letter or first line of an element's content, change the font of the first line of a paragraph, etc.
The syntax for Pseudo Element Selector is selector::pseudo-element { property:value; }. 

::first-letter - Selects the first letter of the text contents inside an element. 
::first-line - Selects the first line of the text contents inside an element. 
::before - Used to insert generated content immediately before an element. 
::after - Used to insert generated content either before or after an element on the page generate content immediately after an element.


![image](https://user-images.githubusercontent.com/12488769/148696175-dd89c65d-1364-4c61-8609-b80ad47fdefb.png)
![image](https://user-images.githubusercontent.com/12488769/148696180-d4364bfb-11d4-4f4d-a3e9-a0738dd33c48.png)

## Specificity in CSS
When we have more than one CSS style rule for an element, the browser selects one style rule for that element based upon a specificity as a score/rank/priority. 
Specificity only applies when the same element is targeted by multiple CSS declarations. 
Specificity is the set of the rules applied to CSS selectors to determine which style is applied to an element. More specific selector will have higher Precedence.
The specificity level of a selector has 4 categories listed below:
Inline CSS - Example: <h1 style="color: #ffffff;"> 
ID Selector
Class Attribute and Pseudo-Classes Selectors.
Element and Pseudo-Elements Selector.
Inline CSS have higher priority and Element and Pseudo-Elements Selector have lowest priority. 





