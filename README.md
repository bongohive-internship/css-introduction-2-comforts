# css-introduction-2 

What you will learn 

### In this section will set:  


- [ ] Header image

- [ ] Nav bar 

> Using basic reset with CSS universal selectors select any type of elements in an HTML page. It matches a single element. An asterisk ( i.e. "*" ) is used to denote a CSS universal selector. An asterisk can also be followed by a selector. This is useful when you want to set a style for of all the elements of an HTML page or for all of the elements within an element of an HTML page. 

**In the main.css file add the following**
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
**The box-sizing CSS property sets how the total width and height of an element is calculated.**


```html
<header class="header">
    hello world
</header>
```

> The inherit CSS keyword causes the element for which it is specified to take the computed value of the property from its parent element. It can be applied to any CSS property, including the CSS shorthand all.

###  Next is importing your font file in your css
 
```
@font-face {
    font-family: "Roboto Regular";
    src: url("../fonts/Roboto-Regular.ttf");
}
```
### Inherit in CSS

>  Using inherit in CSS. We use CSS inherit to have your sitting span over in your all your tags under the tag body. it good practice doing so.

```
body {
    font-family: "Roboto", sans-serif;
    font-weight: 400;
    font-size: 16px;
    line-height: 1.7;
    color: rgb(0, 0, 0);
}
```

 
### Header image 

in your 

````
index.html 
````  
file add the following to your  <header> tag 

```
<header class="header"> No way we did that...  </header>
```

Now back to your 

```
main.css
``` 
file and add in the following class to your CSS 


```
.header { 
    height: 95vh;
    background-image: url(../images/beautiful-blur-bright-326055.jpg);
    background-size: cover;
    background-position: top;
    position: relative;
}
```
At this point you should see your image. 

### Big right? this is because we set our hight to 95vh 
### Feel free to play around with this 

###  Linear-gradient

### "The linear-gradient() CSS function creates an image consisting of a progressive transition between two or more colors along a straight line. Its result is an object of the <gradient> data type, which is a special kind of <image>."

### To do this you will need to add the following on this line

before 
```
background-image: url(../images/beautiful-blur-bright-326055.jpg); 
```

and after 

```
  background-image: linear-gradient(to right bottom,#30303000, #303030b7), url(../images/beautiful-blur-bright-326055.jpg);
```
 
### 6 clip path
### Clipping is when we trim a piece from something. In our case, it is an operation which allows us to completely or partially hide elements on a web page. Two other concepts that relate to clipping which we will use in this article are clipping path and clipping region.

```
clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100% )
```
### Try out other shaps on  https://bennettfeely.com/clippy/


### 7 Adding a logo.png and a div with class 
Back to your

````
index.html 
````  
and add the following in between 

```
<header class="header"> No way we did that...  </header>
```
will add 

```
<header class="header"> 
<div class="logo-box">
        <img src="/images/logo.png" alt="Logo" class="logo">
    </div>
  </header>
```
next we need to position of your loge read up from  

###CSS Layout - The position Property
https://www.w3schools.com/css/css_positioning.asp
```
.logo-box {
    position: absolute;
    top: 40px;
    left: 40px;
    
}

.logo {
    height: 55px;
}
```

### 8


## CSS Resources

### CSS Viewport
### https://www.sitepoint.com/css-viewport-units-quick-start/

### shapes
###  https://bennettfeely.com/clippy/
###  https://www.sitepoint.com/introducing-css-clip-path-property/

### https://developer.mozilla.org/en-US/docs/Web/CSS/inherit

###  css * Selector
### - https://www.w3resource.com/css/selectors/CSS-universal-selector.php

### box-sizing
### - https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing

### - https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Fonts

### how to add custom font 
### - https://www.balbooa.com/knowledgebase/32-documentation-faq-joomla/176-how-to-add-custom-font-to-website-through-fontface
