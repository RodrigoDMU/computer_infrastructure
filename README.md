# Higher Diploma in Science in Computing - Data Analytics
******

## Computer Infrastructure

![Programming](images/img_programming.jpeg)

**by: Rodrigo De Martino Ucedo**
************

# My Assessment Repository

This repository contains my assessment submission for the module of Computer Infrastructure.

## Tasks

**- Task 1: Create Directory Structure:**

**Task description:** Using the command line, create a directory (that is, a folder) named `data` at the root of your repository. Inside `data`, create two subdirectories: `timestamps` and `weather`.

**Summary:** To complete Task 1, I've created the main [`data`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data) directory and I used the `mkdir` command. I also used the `mkdir -p` command to create a data directory with two subdirectories, [`timestamps`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/timestamps) and [`weather`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/weather).

**- Task 2: Timestamps:**

**Task description:** Navigate to the `data/timestamps` directory. Use the `date` command to output the current date and time, appending the output to a file named `now.txt`. Make sure to use the `>>` operator to append (not overwrite) the file. Repeat this step ten times, then use the `more` command to verify that `now.txt` has the expected content.

**Summary:** To complete Task 2, I navigated to the [`data/timestamps`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/timestamps) directory and used the `date` command to append the current date and time to [`now.txt`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/timestamps/now.txt) 10 times. I verified that the data was correctly appended by using the `more` command.

**- Task 3: Formatting Timestamps:**

**Task description:** Run the `date` command again, but this time format the output using `YYYYmmdd_HHMMSS` (e.g., `20241126_130004` for 1:00:04 PM on November 26, 2024). Refer to the date man page (using `man date`) for more formatting options. (Press `q` to exit the man page). Append the formatted output to a file named [`formatted.txt`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/timestamps/formatted.txt).

**Summary:** To complete Task 3, I used the date command with a custom format string to produce the current date and time in the YYYYmmdd_HHMMSS format. I appended the formatted output to a file named formatted.txt using the >> operator and verified the results by viewing the file with the more command.

**- Task 4: Create Timestamped Files:**

**Task description:** Use the `touch` command to create an empty file with a name in the `YYYYmmdd_HHMMSS.txt` format. You can achieve this by embedding your date command in backticks `` ` `` into the touch command. You should no longer use redirection (`>>`) in this step.

**Summary:** To complete Task 4, I used the touch command in combination with the `date` command wrapped in backticks (`` ` ``) to create an file with a timestamped name in the [`YYYYmmdd_HHMMSS.txt`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/timestamps/20241026_132342.txt) format. The `touch` command ensured that the file was created, and the date command dynamically generated the filename based on the current date and time. Finally, I used the `ls` command to verify that the file was created successfully.

**- Task 5: Download Today's Weather Data:**

**Task description:** Change to the `data/weather` directory. Download the latest weather data for the Athenry weather station from Met Eireann using `wget`. Use the `-O <filename>` option to save the file as `weather.json`. The data can be found at this URL: `https://prodapi.metweb.ie/observations/athenry/today`.

**Summary:** To complete Task 5, I navigated to the [`data/weather`](https://github.com/RodrigoDMU/computer_infrastructure/tree/main/data/weather) directory and used the `wget` command to download the latest weather data for the Athenry weather station from the provided [Met Eireann URL](https://prodapi.metweb.ie/observations/athenry/today). I used the `-O` option with wget to save the file as [`weather.json`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/weather/weather.json). Finally, I verified that the file was successfully downloaded by listing the directory contents using the `ls` command.

**- Task 6: Timestamp the Data:**

**Task description:** Modify the command from Task 5 to save the downloaded file with a timestamped name in the format `YYYYmmdd_HHMMSS.json`.

**Summary:** To complete Task 6, I modified the `wget` command from Task 5 by embedding the `date` command within it to generate a timestamped filename. This ensures that the downloaded weather data is saved with a unique filename based on the current date and time in the [`YYYYmmdd_HHMMSS.json`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/weather/20241028_114642.json) format. Finally, I verified the file creation using the ls command to ensure that the timestamped filename was applied correctly.

**- Task 7: Write the Script:**

**Task description:** Write a bash script called `weather.sh` in the root of your repository. This script should automate the process from Task 6, saving the weather data to the `data/weather` directory. Make the script executable and test it by running it.

**Summary:** To complete Task 7, I wrote a bash script called [`weather.sh`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/weather.sh) that automates the process of downloading the latest weather data from Met Eireann and saves it with a timestamped filename. I made the script executable using `chmod +x` and tested it by running the script with `./weather.sh`. Finally, I verified that the weather data was correctly saved in the [`data/weather`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/data/weather/20241108_110531.json) directory with a timestamped filename using the `ls` command. 

**- Task 8: Notebook:**

**Task description:** Create a notebook called `weather.ipynb` at the root of your repository. In this notebook, write a brief report explaining how you completed Tasks 1 to 7. Provide short descriptions of the commands used in each task and explain their role in completing the tasks.

**Summary:** To complete Task 8, I used the `touch` command to create a notebook file named [`weather.ipynb`](https://github.com/RodrigoDMU/computer_infrastructure/blob/main/weather.ipynb) at the root of the repository. After executing the `touch weather.ipynb` command, I verified the file's existence with the `ls` command.

**- Task 9: Pandas:**

**Task description:** In your `weather.ipynb` notebook, use the `pandas` function `read_json()` to load in any one of the weather data files you have downloaded with your script. Examine and summarize the data. Use the information provided [data.gov.ie](https://data.gov.ie/dataset/todays-weather-athenry) to write a short explanation of what the data set contains.

**Summary:** By using `pandas.read_json()` and analyzing the structure of the data, I was able to quickly load and summarize the weather data. The dataset provides valuable insights into daily weather conditions, which can be used for various scientific and practical applications.

## Project







*******
## End