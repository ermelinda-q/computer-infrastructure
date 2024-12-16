# Computer Infrastructure Repository

** by E. Qejvani**
***

## About this Repository.

This git repository contains all the files of Computer Infrastructure module as part of my [Hdip in Computer Science in Data Analytics](https://www.gmit.ie/higher-diploma-in-science-in-computing-in-data-analytics#:~:text=You%20are%20a%20Level%208,topics%20in%20your%20original%20degree.) in [ATU](https://www.gmit.ie/).


## Repository Structure

```
COMPUTER-INFRASTRUCTURE/
|
|-- .github/workflows/        # Contains GitHub Actions workflows
|   |-- weather-data.yml      # Workflow for automating tasks
|
|-- data/                     # Directory for weather data
|   |-- timestamps/           # Subdirectory for timestamp files
|   |-- weather/              # Subdirectory for weather JSON files
|
|-- img/                      # Directory for .png images used in for the tasks and the project
|
|-- .gitignore                # Specifies files and directories to ignore in Git
|-- README.md                 # Documentation for the project
|-- requirements.txt          # Required Python modules for the project
|-- weather.ipynb             # Jupyter Notebook containing tasks and the project
|-- weather.sh                # Automated shell script that runs daily at 20:00
```

## About this Project/Task Assessments.



## Use of this Project.



## Getting Started


## Author

I am a student at [ATU](https://www.atu.ie/).


## Contents

### Tasks
The `weather.ipynb` file includes:
1. **Nine Tasks:** Demonstrating the use of Linux commands and shell scripts in Codespaces.
2. **Project:** Developing an automated shell script to retrieve daily `.json` weather data from the Athenry weather station.

### Workflow
The `.github/workflows/weather-data.yml` file manages automated workflows in this repository, such as running scripts or CI/CD tasks.

### Data
The `data/` directory contains:
- **Timestamps:** Stores timestamp-related files.
- **Weather:** Contains `.json` files of weather data.

### Images
The `img/` directory stores all `.png` files used for visualizations or references.

## Setup and Usage

### Prerequisites
1. Ensure Python 3.8 or later is installed.
2. Install the required modules using the command:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up a Linux environment or use GitHub Codespaces for running shell scripts.
4. Verify that `cron` is installed and running on your system (for daily automation).

### Running the Jupyter Notebook
1. Launch the notebook using the following command:
   ```bash
   jupyter notebook weather.ipynb
   ```
2. Follow the instructions within the notebook to complete tasks and run the project.

### Automating the Shell Script
The `weather.sh` script is scheduled to run daily at 20:00 to retrieve the weather data.

#### Steps:
1. Grant execution permissions to the script:
   ```bash
   chmod +x weather.sh
   ```
2. Add the script to your `crontab` for daily execution:
   ```bash
   crontab -e
   ```
   Add the following line to schedule the script:
   ```
   0 20 * * * /path/to/weather.sh
   ```

### Using GitHub Actions
1. The workflow defined in `.github/workflows/weather-data.yml` automates tasks related to the project.
2. Push changes to the repository to trigger the workflow.

## Contribution
Contributions are welcome. Please follow these steps:
1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request with a detailed description of changes.


### Contact
For queries, please reach out via the ATU communication channels or create an issue in this repository.
