# css-introduction-2 

What you will learn 

### In this section will set 


## - Header image

## - Nav bar 

### using basic reset with CSS universal selectors select any type of elements in an HTML page. It matches a single element. An asterisk ( i.e. "*" ) is used to denote a CSS universal selector. An asterisk can also be followed by a selector. This is useful when you want to set a style for of all the elements of an HTML page or for all of the elements within an element of an HTML page. 

### in the main.css file add the following
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
### The box-sizing CSS property sets how the total width and height of an element is calculated.


```
<header class="header">
hello world
</header>
```

### The inherit CSS keyword causes the element for which it is specified to take the computed value of the property from its parent element. It can be applied to any CSS property, including the CSS shorthand all.

### 2. Next is importing your font file in your css
 
```
@font-face {
    font-family: "Roboto Regular";
    src: url("../fonts/Roboto-Regular.ttf");
}
```
### 3. inherit in CSS

### Using inherit in CSS. To have your sitting span over in your all you tags under body. it good practice doing so.

```
body {
    font-family: "Roboto", sans-serif;
    font-weight: 400;
    font-size: 16px;
    line-height: 1.7;
    color: rgb(0, 0, 0);
}

```

 
### 4. header image 

in your 

````
index.html 
````  
file add the following to your  <header> tag 

```
<header class="header"> No way we did that...  </header>
```

Now back to your 

```main.css
``` 
file and add in the following class to your css 


```
.header { 
    height: 95vh;
    background-image: url(../images/beautiful-blur-bright-326055.jpg);
    background-size: cover;
    background-position: top;
}
```

## css resources

### https://developer.mozilla.org/en-US/docs/Web/CSS/inherit

###  css * Selector
### - https://www.w3resource.com/css/selectors/CSS-universal-selector.php

### box-sizing
### - https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing

### - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Fonts

### how to add custom font 
### - https://www.balbooa.com/knowledgebase/32-documentation-faq-joomla/176-how-to-add-custom-font-to-website-through-fontface