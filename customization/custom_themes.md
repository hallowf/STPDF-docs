---
layout: page
title: Custom Themes
parent: Customization
permalink: /customization/custom-themes/
nav_order: 1
---


## Creating custom themes

1. Duplicate one of the existing themes and rename it to anything you want, just make sure the extension is ".ini" and avoid weird characters 
    - EX:
        * STPDF-mytheme.ini
        * mytheme.ini
        * randomTheme.ini
2. Now open that file with a text editor and just replace the values with your own

**But how does it work ?**

* \[Theme\]
  - Each parameter here takes 3 values RGB (red,gree,blue)
  - values need to be from 0 to 255
  - the commas need to separate the values
    * window=122,122,122

* \[COLOR_EXTRAS\]
  - There are only two possibilities here:
    * lighter <- Makes a lighter shade of the color
    * darker <- Makes a darker shade of the color
      * window=lighter
      * background=darker
  - If you don't want to make it lighter or darker just pass not_defined or undefined
    * window=undefined