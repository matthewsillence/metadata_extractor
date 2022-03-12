# metadata_extractor
## Introduction
This workflow is designed using ABBYY Finereader and Python to capture photographs of printed book title pages, convert to text and parsed using risPy to write out the essential bibliographic metadata as an .ris file, for import into bibliographic management software.

## Image Capture
Take a photograph of the title page of the printed book. This can be done using a mobile phone and importing the image file into ABBYY Finereader's desktop application, or using the mobile app and process the file on a mobile device: https://pdf.abbyy.com/finereader-ios-android/

## Optical Character Recognition (OCR)
Using ABBYY Finereader's OCR functionality, convert the image to a plain text file. Export the .txt file.

## Python Script
Open the Python script in Google Colaboratory, and upload the .txt file in the file driectory.

### Adjusting the Text Case
Read in the .txt file as a string using 'str.capwords()' to capitalise the first letter of each word and convert the remaining letters to lowercase.

### Creating the List
Using the 'split()' function, convert the text string to a list and print the list. To isolate the bibliographic metadata based on positions in the list, assign each list item to a new variable. For example, 'author1' to include last name and first name of the author, 'title' for the title of the work, and 'publisher' for the publisher's details.

## Encoding Text Using risPy
Install and import rispy, and define the entries for type of material, id, primary_title, first_authors, abstract and publisher, inserting the list variables at the relevant fields.

## Exporting to .ris
Creating a new filepath 'export.ris', open the filepath and write out as bibliography_file. To check the contents and fields have been assigned correctly, open the file and read in as data and print.

