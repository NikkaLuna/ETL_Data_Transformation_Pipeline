# ETL Pipeline Extract Transform Load

## Overview
This project demonstrates a simple ETL (Extract, Transform, Load) pipeline implemented in Python. The pipeline extracts data from multiple file formats (CSV, JSON, XML), transforms the data as needed, and then loads the transformed data into a CSV file. The entire process is logged, providing transparency and traceability for each step.

## Features
- **Extraction:** Automatically extracts data from CSV, JSON, and XML files located in the working directory.
- **Transformation:** Converts height from inches to meters and weight from pounds to kilograms, rounding off to two decimal places.
- **Loading:** Saves the transformed data into a CSV file.
- **Logging:** Tracks and logs the progress of the ETL process, including start and end times for each phase.

## Prerequisites
Ensure you have the following installed:

- Python 3.x
- pandas library (install with `pip install pandas`)
- glob (standard Python library, no installation required)
- xml.etree.ElementTree (standard Python library, no installation required)

## Usage

Clone this repository:

```bash
git clone https://github.com/yourusername/etl-pipeline.git
cd etl-pipeline
```

Place your CSV, JSON, and XML files in the same directory as the script.

Run the ETL pipeline:

```bash
python etl_pipeline.py
```

Check the log_file.txt for the ETL process logs and transformed_data.csv for the output.

Logging
The script logs the start and end of each ETL phase to log_file.txt with a timestamp for easier debugging and process tracking.

Output
The transformed data will be saved to transformed_data.csv.