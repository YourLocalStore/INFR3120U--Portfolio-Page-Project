Second-Year Web & Script Programming Assignment for IT

# Welcome to my Portfolio Page!
Here, I will explain many of the details that went into my page, such as:

- [Viewports](#viewport-choices);
- [Linear/Angled Gradient Choices](#gradient-choices); and
- [Color Schemes](#color-scheme-choices)

As a quick note, this portfolio is also being deployed on [Github Pages](https://yourlocalstore.github.io/INFR3120U--Portfolio-Page-Project/).

**All** HTML formatting and CSS styling has been written by me, only with the help of course lectures and documentation.
Furthermore, most of the images used in this portfolio are taken by me, while some are fairly used under [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page).
###### * Citations can be found by [clicking here](#citations)

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
###### ** Disclaimer that all pixel widths are tested on a desktop environment, using DevTools to see how specific devices fit and respond to my webpage.

### Viewport #1 - Fully-Sized Screens (Desktops, Laptops, etc..)
The reason why I use at least a minimum portrait width of ```960px``` is because that is how all the content of my page is measured across. This accounts for my main page wrapper, which is specified to hold that fixed width.

```css
#page-wrapper{
    width:  960px;
    min-height: 1024px;
    ...
}
```

In order to have the full experience of my design, I needed any device >= ```960px``` in viewport width. You also find that many other devices (like tablets, especially older ones, or foldable phones) seem to fall below or under
that threshold, especially after testing devices like the ```iPad Mini, Galaxy Z Fold 5/6, Surface Pro 10, etc.,``` within DevTools. 

### Viewport #2 - Tablets
I use at least a minimum portrait width of ```480px``` and a maximum portrait width of ```959px``` to both follow from the constraints of **Viewport #1**, as well as accounting for foldable devices (e.g., the Surface Duo, which measures ```540px``` for one side)
and the devices mentioned in **Viewport 1**. 

Arguably while these devices also fall under the smartphone category, having the extra screen extends that viewport width even further, even past ```480px``` and ```960px```, so a "middle" breakpoint is necessary. 
Another point I want to note is to also accommodate for many of the older devices that have a viewport width larger than ```480px```, so they do not get categorized for "smartphone width", which leaves smaller elements on the page.

### Viewport #3 - Smartphones
The maximum width of ```479px``` was to again follow along with the constraints of **Viewport 2**, but also, many smartphones, even one of the newer [iPhone models](https://www.webmobilefirst.com/en/devices/apple-iphone-18-pro-max-2026/) have a viewport width decently under ```480px```. 
From my overall testing in DevTools, it also seemed as though many of these smartphones fell under this threshold, with about half of them sitting around ```~400px``` in viewport width.

# Gradient Choices
There are only two instances where I use a linear gradient and an angled linear gradient within my website.

### Instance 1 - Linear Gradient to Cover the Whole Page
This linear gradient is used throughout all my website pages, and is colored to fit in with my color scheme. It is behind all body, header, and footer content.
```css
body{
    background-image: linear-gradient(to bottom, #2E3E50, #E0E0E0);
    ...
}
```
![Image](https://github.com/YourLocalStore/INFR3120U--Portfolio-Page-Project/blob/main/linear-gradient-page.png)

### Instance 2 - Angled Linear Gradient for a Header Image
This angled linear gradient uses a parameter of 90 degrees (clockwise) as an aesthetic/design choice to make my image within the top header to stand out a little more using contrast. It will be seen throughout all of my pages.
In the case the visitor has a small enough viewport (i.e., Viewport #3 for Smartphones), both the image and gradient disappear.
```css
#banner-wrapper .header-image img{
    background-image: linear-gradient(90deg, #2E3E50 50%, #E0E0E0 50%);
    ...
}
```
![Image](https://github.com/YourLocalStore/INFR3120U--Portfolio-Page-Project/blob/main/angled-linear-gradient-page.png)

# Color Scheme Choices
Four colors were used in this page, though the course states at least five colors are recommended, I thought it was enough for my page, especially with so many elements squeezed into one 960px wrapper (excluding the footer), it would have otherwise
created some visual clutter. These four colors (in their respective hex format) are:
- #D94A64 (Warm Red)
- #2B7DA4 (Azure)
- #2E3E50 (Dark Azure)
- #E0E0E0 (Light, White-ish Gray)

An insight to their purpose is also written out below.
![Image](https://github.com/YourLocalStore/INFR3120U--Portfolio-Page-Project/blob/main/page-color-scheme.png)

An insight to the colors, and their purpose:
- #D94A64 (Warm Red), is mainly used for nagivation, so it's easier for visitors to see what header they are reading under, or specific buttons on the page.
- #2B7DA4 (Azure), which is used as a background for the images scattered throughout the site. It is meant to create lighter contrast between the background (which uses #2E3E50), and the image itself.
- #2E3E50 (Dark Azure), used as a background color.
- #E0E0E0 (Light, White-ish Gray), which has the same purpose as #2E3E50, but is also used for border coloring for separation and as a text color between elements.

###### Displayed below is an example from the home page.
![Image](https://github.com/YourLocalStore/INFR3120U--Portfolio-Page-Project/blob/main/color-scheme-example.png)

# Citations
Cisco. (n.d.-a). File:cisco logo blue 2016.SVG. Wikimedia Commons. 
https://commons.wikimedia.org/wiki/File:Cisco_logo_blue_2016.svg

Clover, A. (n.d.). File:python windows source code icon 2006–2016.SVG. Wikimedia Commons. 
https://commons.wikimedia.org/wiki/File:Python_Windows_source_code_icon_2006%E2%80%932016.svg 

RISC-V Foundation. (n.d.). File:RISC-V-logo-square.svg. Wikimedia Commons. 
https://commons.wikimedia.org/wiki/File:RISC-V-logo-square.svg 

