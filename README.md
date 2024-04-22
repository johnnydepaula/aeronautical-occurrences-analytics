# Aeronautical Occurrences Analytics
#### Project Status: <font color="orange"> In Progress </font>

## 1. Introduction

---
This project is part of a series of dedicated studies in the field of `Data Engineering and Analytics`,
where I aim to apply data engineering and analytics techniques to analyze data in its various forms and from any source.
My main goal is to replicate real-world scenarios and develop a portfolio of projects that will extend my knowledge and
skills in the field.

I also aim to turn this repository into a crash-course for beginners in the field of data engineering and analytics,
and present a step-by-step guide on how to approach data projects, from data extraction
to data visualization, and I intend to present this as a course at the Academic Week of the Federal Institute
where I currently study.


## 2. Overview

---
### 2.1. Objective
The primary objective of this project is `create a data pipeline` that extracts data from Brazil's public data API,
loads raw data into a S3-like bucket (we'll talk more about this later on), transform and move the processed data to
an analytical directory inside our S3-like bucket. Once all this process is done, we'll try to `orchestrate` each one
of these single steps into a `DAG`, using `apache airflow`. 

### 2.2. Topics

* `Data Extraction`
* `Data Manipulation`
* `Amazon S3 Concepts`
* `Job Orchestration`
* `Data Ingestion`

### 2.3. Technologies
* `Jupyter`
* `Python`
* `SQLite`
* `Airflow`


## 3. Getting Started

---
Instructions on how to set up the project, including installing dependencies, setting up the database, and running the code.

### 3.1. Dependencies

---
To run this project, you'll need some libraries on your machine. As a good practice, I recommend setting up a virtual 
environment to avoid possible conflicts between libraries you could already have installed on your machine. To do so,
you can use `venv` or `conda` to create a new environment.
If using python virtual environment, you can create a new environment by running the following command:

`python -m venv <env_name>`

and then activate the environment by running:

`source <env_name>/bin/activate`


To makes this process easier, there's a `requirements.txt`
file in the root directory of this project. You can install all the dependencies by running the following command:

`pip install -r requirements.txt`

or you can install them individually by running `pip install pandas jupyter ...`, for any other library you want to use
if importing or testing the code.

If you're using `conda`, you can create a new environment and install the dependencies by running the following command:

`
conda create --name <env_name> --file requirements.txt
`.

Make sure that you've installed ati least `python3.8`, `jupyter`, `pandas` and `sqlite` on your machine. We'll talk about
airflow installation and configuration later on



## 4. Roadmap

---
* [x] Extract from Brazil's public data API
* [x] Load raw data into a S3-like bucket
  * [x] Create `{key : pair}` values to access the files and its metadata (optional)
* [ ] Perform data transformation
  * [ ] Clean the data
  * [ ] Create new columns
  * [ ] Aggregate data
  * [ ] Create a new dataset
* [ ] Return processed data to our S3-like bucket
* [ ] Load the processed data into a SQLite database
* [ ] Orchestrate the entire process using Apache Airflow

## Data
Description of the data used in the project, including its source, the format, and any preprocessing steps taken.

## Methodology
Detailed description of the methods and techniques used in the project, including data extraction, manipulation, and visualization.

## Results
Summary of the results obtained, including any patterns, trends, or correlations identified.

## Future Work
Description of any planned future work for the project.

## Contributing
Information on how others can contribute to the project.

## License
Information about the project's license.
