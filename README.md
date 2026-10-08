Second-Year Web & Script Programming Assignment for IT

# Welcome to my Portfolio Page!
Here, I will explain many of the details that went into my page, such as:

- [Viewports](#viewport-choices);
- [Linear/Angled Gradient Choices](#gradient-choices); and
- [Color Schemes](#color-scheme-choices)

As a quick note, this portfolio is also being deployed on [Github Pages](https://yourlocalstore.github.io/INFR3120U--Portfolio-Page-Project/).

**All** HTML formatting and CSS styling has been written by me, only with the help of course lectures and documentation.
Furthermore, most of the images used in this portfolio are taken by me, while some are fairly used under [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page).
###### * Citations can be found by clicking here

# Viewport Choices
At the very start of my HTML files, I put the necessary queries under the ```<head>``` tag. This is done so that my media queries will be loaded across all pages of my portfolio in order to implement fully responsive design.
Attached below, are the media queries I use:
```html
<!-- Computers or any device >= 960px in viewport width 
     The maximum width is either 960px or above.
-->
<link rel="stylesheet" 
      type="text/css" 
      href="./CSS/homestyle.css"
      media="only screen and (min-width:960px)"> 
    
<!-- Tablets or any device > 480px and < 960px in viewport width 
     The maximum width is 959px.
-->
<link rel="stylesheet" 
      type="text/css" 
      href="./CSS/tablet.css"
      media="only screen and (min-width:480px) and (max-width: 959px)">

<!-- Computers or any device < 480px in viewport width 
     The maximum width is 479px.
-->
<link rel="stylesheet" 
      type="text/css" 
      href="./CSS/smartphone.css"
      media="only screen and (max-width:479px)">
```
###### ** Disclaimer that all pixel widths are tested on a Desktop environment, using DevTools to see how specific devices fit and respond to my webpage.

### Viewport #1 - Fully-Sized Screens (Desktops, Laptops, etc..)
The reason why I use at least a minimum portrait width of ```960px``` is because that is how all the content of my page is measured across. This accounts for my main page wrapper, which is specified to hold that fixed width.

In order to have the full experience of my design, I needed any device >= ```960px``` in viewport width. You also find that many other devices (like tablets, especially older ones, or foldable phones) seem to fall below or under
that threshold, especially after testing devices like the ```iPad Mini, Galaxy Z Fold 5/6, Surface Pro 10, etc.,``` within DevTools. 

### Viewport #2 - Tablets
I use at least a minimum portrait width of ```480px``` and a maximum portrait width of ```959px``` to both follow from the constraints of **Viewport #1**, as well as accounting for foldable devices (e.g., the Surface Duo, which measures ```540px``` for one side). 

Arguably while these devices also fall under the smartphone category, having the extra screen extends that viewport width even further, even past ```480px``` and ```960px```, so a "middle" breakpoint is necessary. 
Another point I want to note is to also accommodate for many of the older devices that have a viewport width larger than ```480px```, so they do not get categorized for "smartphone" width, which leaves smaller elements on the page.

### Viewport #3 - Smartphones
The maximum width of ```479px``` was to again follow along with the constraints of **Viewport 2**, but also, many smartphones, even one of the newer [iPhone models](https://www.webmobilefirst.com/en/devices/apple-iphone-18-pro-max-2026/) have a viewport width decently under ```480px```. 
From my overall testing in DevTools, it also seemed as though many of these smartphones fell under this threshold, with about half of them sitting around ```~400px``` in viewport width.

# Gradient Choices
There are only two instances where I use a linear gradient and an angled linear gradient within my website.

### Instance 1 - Linear Gradient to Cover the Whole Page
```css
body{
    background-image: linear-gradient(to bottom, #2E3E50, #E0E0E0);
    ...
}
```

### Instance 2 - Angled Linear Gradient for a Header Image
```css
#banner-wrapper .header-image img{
    background-image: linear-gradient(90deg, #2E3E50 50%, #E0E0E0 50%);
    ...
}
```



# Color Scheme Choices
colors!
