# Higher Diploma in Science in Computing - Data Analytics
******

## Computer Infrastructure

![Programming](images/img_programming.jpeg)

**by: Rodrigo De Martino Ucedo**
************

# My Assessment Repository

This repository contains my assessment submission for the module of Computer Infrastructure.

## Getting Started

**- Task 1: Create Directory Structure:**

**Task description:** Using the command line, create a directory (that is, a folder) named `data` at the root of your repository. Inside `data`, create two subdirectories: `timestamps` and `weather`.

**Summary:** To complete Task 1, I've created the main [`data`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data) directory and I used the `mkdir` command. I also used the `mkdir -p` command to create a data directory with two subdirectories, [`timestamps`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/timestamps) and [`weather`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/weather). The `-p` option allowed me to create the necessary directory structure in a single command, ensuring that all the required directories were in place for the next tasks.

**- Task 2: Timestamps:**

**Task description:** Navigate to the `data/timestamps` directory. Use the `date` command to output the current date and time, appending the output to a file named `now.txt`. Make sure to use the `>>` operator to append (not overwrite) the file. Repeat this step ten times, then use the `more` command to verify that `now.txt` has the expected content.

**Summary:** To complete Task 2, I navigated to the [`data/timestamps`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/timestamps) directory and used the `date` command to append the current date and time to [`now.txt`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/timestamps/now.txt) 10 times. I verified that the data was correctly appended by using the `more` command.

**- Task 3: Formatting Timestamps:**

**Task description:** Run the `date` command again, but this time format the output using `YYYYmmdd_HHMMSS` (e.g., `20261114_130003` for 1:00:03 PM on November 14, 2026). Refer to the date man page (using `man date`) for more formatting options. (Press `q` to exit the man page). Append the formatted output to a file named `formatted.txt`.

**Summary:** To complete Task 3, I used the date command with a custom format string to produce the current date and time in the YYYYmmdd_HHMMSS format. I appended the formatted output to a file named formatted.txt using the >> operator and verified the results by viewing the file with the more command.

**- Task 4: Create Timestamped Files:**

**Task description:** Use the `touch` command to create an empty file with a name in the `YYYYmmdd_HHMMSS.txt` format. You can achieve this by embedding your date command in backticks `` ` `` into the touch command. You should no longer use redirection (`>>`) in this step.

**Summary:**

**- Task 5: Download Today's Weather Data:**

**Task description:** Change to the `data/weather` directory. Download the latest weather data for the Athenry weather station from Met Eireann using `wget`. Use the `-O <filename>` option to save the file as `weather.json`. The data can be found at this URL: `https://prodapi.metweb.ie/observations/athenry/today`.

**Summary:**

**- Task 6: Timestamp the Data:**

**Task description:** Modify the command from Task 5 to save the downloaded file with a timestamped name in the format `YYYYmmdd_HHMMSS.json`.

**Summary:**

**- Task 7: Write the Script:**

**Task description:** Write a bash script called `weather.sh` in the root of your repository. This script should automate the process from Task 6, saving the weather data to the `data/weather` directory. Make the script executable and test it by running it.

**Summary:**

