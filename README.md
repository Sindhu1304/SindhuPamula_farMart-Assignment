# SindhuPamula_farMart-Assignment
# Log Extraction from Large File

This repository contains a solution for efficiently extracting log entries from a large log file (approximately 1 TB in size) based on a specified date. The solution reads the log file line by line to avoid memory overload and extracts all log entries for a given date. It then saves these logs to a separate output file.

## Problem Statement

You are tasked with extracting log entries from a large file containing logs generated over multiple years. The file format consists of a timestamp, log level, and message. The goal is to extract all logs for a specific date, using minimal memory and ensuring efficiency.

### Log Format Example:

