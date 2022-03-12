# metadata_extractor
## Introduction
This workflow is designed using ABBYY Finereader and Python to capture photographs of printed book title pages, convert to text and parsed using risPy to write out the essential bibliographic metadata as an .ris file, for import into bibliographic management software.

## Image Capture
Take a photograph of the title page of the printed book. This can be done using a mobile phone and importing the image file into ABBYY Finereader's dektop application, or using the mobile app and process the file on a mobile device.

## Optical Character Recognition (OCR)
Using ABBYY Finereader's OCR functionality, convert the image to a plain text file. Export the .txt file.

## Python Script
Open the Python script in Google Colaboratory, and upload the .txt file in the file driectory.

### Adjusting the Text Case
Read in the .txt file as a string using 'str.capwords()' to capitalise the first letter of each word and convert the remaining letters to lowercase.

### Creating the List
Using the 'split()' function, convert the text string to a list and print the list. To isolate 

