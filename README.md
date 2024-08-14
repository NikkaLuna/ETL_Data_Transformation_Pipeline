# ETL Data Transformation Pipeline

## Overview
This project demonstrates a simple ETL (Extract, Transform, Load) pipeline implemented in Python. The pipeline extracts data from multiple file formats (CSV, JSON, XML), transforms the data, and then loads the transformed data into a CSV file. The entire process is logged, providing transparency and traceability for each step.

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

1. **Clone the Repository:**
   
```bash
git clone https://github.com/NikkaLuna/ETL_Data_Transformation_Pipeline.git
cd ETL_Data_Transformation_Pipeline
```
2. **Set Up the Environment:**
   
   Ensure you have Python 3.x installed on your system.
   
   *(Optional but recommended)* Create and activate a virtual environment to manage dependencies:

```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. **Install Dependencies:**
   
   Install the required Python packages. Since some packages are part of the standard library (like `glob` and `xml.etree.ElementTree`), you only need to install `pandas`:

```bash
pip install pandas
```

4. **Place Your Data Files:**
Place your CSV, JSON, and XML files in the same directory as the etl_pipeline.py script. Ensure that these files are correctly formatted as expected by the script.

5. **Run the ETL Pipeline:**
Execute the script to run the ETL process:

```bash
python etl_pipeline.py
```


## Logging
The script logs the start and end of each ETL phase to log_file.txt with a timestamp for easier debugging and process tracking.

## Output
The transformed data will be saved to transformed_data.csv.
