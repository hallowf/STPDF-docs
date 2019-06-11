---
layout: page
title: Installing tesseract
parent: Help
permalink: /help/tesseract/
nav_order: 1
---

## Windows

1. So first you grab an installer from [here](https://github.com/UB-Mannheim/tesseract/wiki)
 * Download the one that fits your machine 32bit/64bit

2. Go trough the installer and if you would like it to work with more languages download the additional language packs
    * <div style="text-align: center"><img style="display: inline-block; width: 400px; height: 300px" src="/STPDF-docs/assets/imgs/tesseract-langs.png"></div>

3. Then it will ask you where to install it is important you remember the location you will need it for later
    * I installed mine to C:\Tesseract-OCR but you can choose the default location, just note it down

    * <div style="text-align: center"><img style="display: inline-block; width: 400px; height: 300px" src="/STPDF-docs/assets/imgs/tesseract-install.png"></div>

4. Now you will need to add it to your PATH environment variable
 * Open the windows menu, right click on "computer" left click on properties
 * Then on your right should be Advanced system settings, click there
 * A new window should appear, click on Environment Variables
 * A new window should appear again, on the top are your user environment variables
 * Locate on that top part the PATH variable click on it and select edit
 * Now where it says value of the variable be carefull to not delete stuff might break other apps,
 simply press the end key (or use the arrows) and you should be at the end
 * Now you add ";TESSERACT_PATH", where TESSERACT_PATH is the install location, don't forget the semicolon before
 * You might need to restart your system or refresh your environment, but after this you should be able to call tesseract from the command line

5. Verify it is installed

    * <div style="text-align: center"><img style="display: inline-block; width: 600px; height: 300px" src="/STPDF-docs/assets/imgs/tesseract-installed.gif"></div>

## Debian

1. <code>sudo apt install tesseract-ocr -y</code>
2. verify it is installed ...