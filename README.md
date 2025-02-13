# SindhuPamula_farMart-Assignment
# Log Extraction from Large File

This repository contains a solution for efficiently extracting log entries from a large log file (approximately 1 TB in size) based on a specified date. The solution reads the log file line by line to avoid memory overload and extracts all log entries for a given date. It then saves these logs to a separate output file.

## Problem Statement

You are tasked with extracting log entries from a large file containing logs generated over multiple years. The file format consists of a timestamp, log level, and message. The goal is to extract all logs for a specific date, using minimal memory and ensuring efficiency.

### Log Format Example:

Each log entry starts with a timestamp (`YYYY-MM-DD HH:MM:SS`), followed by the log level (e.g., `INFO`, `ERROR`, `WARN`), and a message.

## Features

- **Efficient Memory Usage**: The solution reads the file line by line, ensuring minimal memory usage even for large log files (up to 1 TB).
- **Flexible Date Filtering**: Users can specify any date in the `YYYY-MM-DD` format, and the program will filter the logs accordingly.
- **Output File Creation**: Extracted logs are saved to a new file named `output_YYYY-MM-DD.txt` in the same directory.
- **Error Handling**: The script includes basic error handling to manage file-related issues and unexpected errors.

## Prerequisites

- **Python 3.x**: Ensure that Python 3.x is installed on your system.
- **Google Colab (Optional)**: While the solution can run on any local Python environment, you can use Google Colab for running the script in the cloud and avoiding local setup issues.
- **Log File**: The log file (e.g., `logs_2024.log`) should be in `.log` format.

## Installation

1. Clone this repository to your local machine or fork it to your GitHub account:

    ```bash
    git clone <repository_url>
    ```

2. Ensure you have Python 3.x installed on your local machine, or use Google Colab for cloud execution.

3. Upload your log file (e.g., `logs_2024.log`) to Google Colab or use it directly on your local machine.

## How to Run the Script

### Option 1: Running the Script in Google Colab

1. **Upload the Log File**: Upload your log file (`logs_2024.log`) to Google Colab using the following code snippet:

    ```python
    from google.colab import files
    uploaded = files.upload()
    ```

2. **Run the Script**: Run the extraction script with the desired date as a command-line argument. For example, to extract logs for `2024-12-01`, run the following in Colab:

    ```bash
    !python extract_logs.py 2024-12-01
    ```

3. **Download the Output**: After the logs are extracted, download the result using the following code:

    ```python
    from google.colab import files
    files.download('/content/output_2024-12-01.txt')
    ```

### Option 2: Running Locally on Your Machine

1. **Prepare the Log File**: Place the log file (e.g., `logs_2024.log`) in the same directory as the Python script or provide the full path to the file.

2. **Run the Script**: Open a terminal or command prompt and run the script with the desired date:

    ```bash
    python extract_logs.py 2024-12-01
    ```

3. **Check the Output**: The extracted logs will be saved in a file named `output_2024-12-01.txt` in the current working directory.

## Example Usage

### Example 1: Extract Logs for `2024-12-01`

To extract logs for December 1, 2024, run the following command:

```bash
python extract_logs.py 2024-12-01


