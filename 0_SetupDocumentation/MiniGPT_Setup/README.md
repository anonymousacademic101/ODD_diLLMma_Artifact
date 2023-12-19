# MiniGPT

To run this code please download and install [https://minigpt-4.github.io/](https://minigpt-4.github.io/). You can then use the code in `CustomCode` to run the models on large volumes of data without the need for a GUI interface.


# MiniGPT4 Setup

This README guides you through setting up and running the MiniGPT4 model for processing large volumes of data with Vicuna and Llama 2.

## Prerequisites
Commit Version: Ensure you are using commit X of MiniGPT4 for compatibility.
Hardware Requirements: List the minimum and recommended hardware specifications.
Graphics Drivers: Specify the graphics drivers used during development.
Python Environment: Python version (e.g., Python 3.8) and any other relevant environment details.


## Installation
Download MiniGPT4:

Visit MiniGPT4 Official Page and download the relevant files.
Install Requirements:

Navigate to the MiniGPT4 directory.
Install dependencies using the provided requirements.txt file:
bash
Copy code
pip install -r requirements.txt


## Directory Structure
Set up your working directory as follows:

MiniGPT4/
CustomCode/ (Place your custom scripts here)
Data/ (Your dataset goes here)
Models/ (Model files from MiniGPT4)
... (other MiniGPT4 directories and files)


## Running the Code
To run the custom code on your dataset:

Place your dataset in the Data/ directory.
Navigate to the CustomCode/ directory.

Run the custom script:
```bash
Copy code
python run_minigpt4.py --data ../Data/your_dataset.csv
```

Example Usage and Output
Command:
bash
Copy code
python run_minigpt4.py --data ../Data/sample_data.csv
Expected Output:
Describe the expected console output or results.
Include a screenshot of the expected output for clarity.
Troubleshooting
Provide common issues and their solutions.
Contact information for further assistance.


./run_model.sh vicuna OpenPilot_utah 1
