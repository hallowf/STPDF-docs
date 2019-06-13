---
layout: page
title: titles.stpdf_core
parent: Usage
permalink: /usage/stpdf-core/
nav_order: 3
---

### Under the hood

So The first thing the "core-module" does after you've passed your input trough the GUI or CLI is check the number of files in the source directory and subsequent folders

Then it starts to "process" them one by one and what is this process?

1. First it creates a list(list1) of all files in the directory

2. Now for each file in the list1
  * If the file has a know extension(PNG,JPG) then read it into a list(list2) in memory:
    - If deskew(remove rotation) is true then
      * Get the output rotation from tesseract providing the image in list2
      * Rotate the image and overwrite the old one in memory
      * If save files is true then it saves it to the output directory and skips to the next image in list1
    - Else
      * Append the image to the list2
      * And once again if save files is true it saves it to the output directory

3. Final step is to make a pdf
    * For image in list2
    * If split into multiple PDF's is true
      - Modify the list into a list(list2 but modified) of lists with the image handles
      - For list in list2
        * Get the first item/image in the list and save it as a PDF
        * Remove that entry from the list and append all the other images to the PDF


#### But do you need all these steps?

Some are optional and disabling might help speed up the whole process, let's say: 
1. you only want to deskew images
  * then disable make pdf in the gui
2. you only want the PDF(s) not the rotated images
  * then disable image copy
  
you can learn more about this in [App performance](../../help/app-performance/)