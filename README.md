## My Computer Infrastructure Assessment Repository

** by E. Qejvani**

This repository contains my assessment submission for the Computer Infrasturcture Module.

## Getting Started


## Purpose of the Assessment.

The purpose of the assessment is to demonstrate ability in the following:

- Use, configure, and script in a command line interface environment.

- Manipulate and move data and code using the command line.

- Compare commonly available software infrastructures and architectures.

- Select appropriate infrastructure for a given computational task.


## Tasks to complete this Assessment.

_Task 1: Create Directory Structure_
Using the command line, create a directory (that is, a folder) named data at the root of your repository. Inside data, create two subdirectories: timestamps and weather.

_Task 2: Timestamps_
Navigate to the data/timestamps directory. Use the date command to output the current date and time, appending the output to a file named now.txt. Make sure to use the >> operator to append (not overwrite) the file. Repeat this step ten times, then use the more command to verify that now.txt has the expected content.

_Task 3: Formatting Timestamps_
Run the date command again, but this time format the output using YYYYmmdd_HHMMSS (e.g., 20261114_130003 for 1:00:03 PM on November 14, 2026). Refer to the date man page (using man date) for more formatting options. (Press q to exit the man page). Append the formatted output to a file named formatted.txt.

_Task 4: Create Timestamped Files_
Use the touch command to create an empty file with a name in the YYYYmmdd_HHMMSS.txt format. You can achieve this by embedding your date command in backticks ` into the touch command. You should no longer use redirection (>>) in this step.

_Task 5: Download Today's Weather Data_
Change to the data/weather directory. Download the latest weather data for the Athenry weather station from Met Eireann using wget. Use the -O <filename> option to save the file as weather.json. The data can be found at this URL:
https://prodapi.metweb.ie/observations/athenry/today.

_Task 6: Timestamp the Data_
Modify the command from Task 5 to save the downloaded file with a timestamped name in the format YYYYmmdd_HHMMSS.json.

_Task 7: Write the Script_
Write a bash script called weather.sh in the root of your repository. This script should automate the process from Task 6, saving the weather data to the data/weather directory. Make the script executable and test it by running it.

_Task 8: Notebook_
Create a notebook called weather.ipynb at the root of your repository. In this notebook, write a brief report explaining how you completed Tasks 1 to 7. Provide short descriptions of the commands used in each task and explain their role in completing the tasks.

_Task 9: pandas_
In your weather.ipynb notebook, use the pandas function read_json() to load in any one of the weather data files you have downloaded with your script. Examine and summarize the data. Use the information provided data.gov.ie to write a short explanation of what the data set contains.