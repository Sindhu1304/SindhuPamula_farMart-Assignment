# SindhuPamula_farMart-Assignment
# Log Extraction from Large File

This repository contains a solution for efficiently extracting log entries from a large log file (approximately 1 TB in size) based on a specified date. The solution reads the log file line by line to avoid memory overload and extracts all log entries for a given date. It then saves these logs to a separate output file.

## Problem Statement

You are tasked with extracting log entries from a large file containing logs generated over multiple years. The file format consists of a timestamp, log level, and message. The goal is to extract all logs for a specific date, using minimal memory and ensuring efficiency.

### Log Format Example:

Each log entry starts with a timestamp (`YYYY-MM-DD HH:MM:SS`), followed by the log level (e.g., `INFO`, `ERROR`, `WARN`), and a message.

2024-12-01 14:23:45 INFO User logged in 2024-12-01 14:24:10 ERROR Failed to connect to the database 2024-12-02 09:15:30 WARN Disk space running low

perl
Copy
Edit









