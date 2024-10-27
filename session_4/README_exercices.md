# Session 4 exercices
# Overview

This project analyzes a collection of annotation files stored in a folder, each with a specific naming convention. The goal was to gather insights from these files, such as the total count, those following a specified format, monthly distribution, and unique identifiers. Each file is structured with specific fields, including date, time, satellite number, version, and a unique region code.
 
# Objectives

The main objectives of this project were:

1. How many files the annotations folder has.
2. How many of them follow the name convention expressed above.
3. How many of annotations you have per month and year. Which month has more annotation files.
4. Create a new annotations folder with multiple folders corresponding to a month.
5. Print all the annotations from the most recent to the oldest one. 
6. How many different satellites there are, how many annotations we have per satellite number, and which one was used in the most recent annotation file. 
7. How many unique regions there are.

The solution was implemented step-by-step in Python, using standard libraries such as os, glob, and shutil for file handling. Here’s a summary of each part:

- File Count: Used glob to get all files in the folder and count them.
- Naming Convention Check: Split each filename and validated each part (date, time, satellite number, etc.) to see if it matches the required format.
- Monthly Annotations: Extracted the year and month from each file, counted occurrences, and determined the busiest month.
- Folder Organization: Created a new structure to organize files by year and month for easy access.
- Sorting: Sorted files by date to display them in descending order.
- Satellite and Region Analysis: Extracted unique satellite numbers and regions and counted them, then found the latest file per satellite.

# Results

- Total files: 206
- Files following the naming convention: 195
- Unique satellites: 5
- Unique regions: 146
- Month with the most annotations: April 2023
