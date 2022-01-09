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





