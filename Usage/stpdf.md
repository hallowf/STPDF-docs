---
layout: page
title: STPDF-GUI
parent: Usage
permalink: /usage/stpdf/
nav_order: 1
---

## Usage

### How it works
You will need to provide it with the directory of all the scans, and a directory to copy the files over,
STPDF does not touch your original files so make sure you have the required disk space.

Then the app starts searching trough that directory and subsequent folders,
when it finds an image, if deskew is checked, the image is rotated and saved directly to the destination
if not it makes a list of all images to copy and copies them over

### About the parameters

1. Source: Directory dialog <- This is the location of your scans
2. Destination: Directory dialog <- The destination to copy the files over
3. Deskew: checkbox <- Removes rotation from your scans, this requires tesseract it will be locked if you don't have it on your system
4. Split scans: checkbox <- This allows you to split your scans into multiple PDF's
5. Split at: slider <- Defines how many scans per PDF
6. Show values: button <- Shows all your current  values and settings
7. Clean log: button <- Cleans the log on the right side
8. Run: button <- Starts STPDF-core


### Menu

* App
    * Save <- Saves your settings, shortcut ("ctrl+s")
    * Exit <- Exit the app

* Options
    * Settings <- Opens settings window, shortcut ("ctrl+o")
    * Help/About <- Link to this docs


### Settings

1. Language <- Language of the app
2. Theme <- Theme of the app
3. Console log level <- This is only for debugging purposes
4. Keep values <- Stores your parameters, Source, Dest, etc, in a file and loads it on startup
5. Apply settings <- This saves your settings if you make changes and close the window before applying your changes, they will be discarded