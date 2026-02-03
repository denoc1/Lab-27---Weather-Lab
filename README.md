# Lab-27---Weather-Lab

## Overview
In this lab, you will practice reading data from a file, storing that data in objects, and performing calculations using an array of objects.

You are given a file containing daily weather data.  
Each line in the file represents **one day**.

Your job is to:
1. Put the data in the folder as a tab-separated-values files
2. Create a class to represent one day of weather data
3. Read the data from the file
4. Store the data in an array
5. Perform simple calculations on the data

---

## The Data File - located on Blackbaud

The file contains:
- A header row
- 40 days of weather data

Each row has:
- `Day` (int)
- `Temp` (double)
- `Precip` (double)

---

## Part 1: Create the `WeatherDay` Class

Create a class called `WeatherDay` with:

### Instance Variables

### Constructor
The constructor should initialize all three instance variables.

### Accessor Methods
Provide at least:
- `getTemperature()`
- `getPrecipitation()`
- `toString()`
(No mutators are needed.)

---

## Part 2: Read the File and Store the Data

In your main program:

1. Create a `Scanner` to read from `weather.txt`
2. Skip the header row
3. Read each day’s data
4. Create a `WeatherDay` object for each row
5. Store the objects in an array

You may assume:
- The file contains **exactly 40 days**
- The file is formatted correctly

---

## Part 3: Data Analysis

Using the array of `WeatherDay` objects, compute and display:

### Required Calculations
1. **Average temperature** for all 40 days  
2. **Total precipitation** for all 40 days  
3. **Number of days with temperature ≥ 50°F**  
4. **Highest temperature recorded**

Print each result with a clear label.

---
          ### Summary Statistics
          - **Total number of days:** 40  
          - **Average temperature:** 67.9°F  
          - **Total precipitation:** 4.15 inches  
          - **Number of rainy days (precipitation > 0):** 13  



## Challenge Extension 1 (Optional): Longest Warm Streak

If you finish the required parts of the lab early, complete the following challenge.

A **warm day** is defined as a day where the temperature is **greater than or equal to 60°F**.

### Task
Determine the **longest consecutive streak of warm days** in the data.

Your program should calculate and display:
- The length of the longest warm streak (number of days)

### Notes
- The streak must consist of **consecutive days**
- If a day is below 60°F, the current streak ends
- You will need to keep track of:
  - the current streak length
  - the longest streak found so far

Do **not** hardcode values. Use a loop to analyze the data.


## Challenge Extension 2 (Optional):  Average temp during longest warm streak

After determining the longest warm streak:

1. Calculate the **average temperature during the longest warm streak**.
2. Display this value along with the length of the streak.

Notes:
- The average should include **only** the days that are part of the longest warm streak.
- You may assume there is only one longest warm streak in the data.
- This calculation should be done **after** the longest streak has been identified.
