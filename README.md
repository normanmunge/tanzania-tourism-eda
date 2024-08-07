# Data Wrangling/Munging to analyze Tourism in Tanzania

The Tanzanian tourism sector plays a significant role in the Tanzanian economy, contributing about 17% to the country’s GDP and 25% of all foreign exchange revenues. The sector, which provides direct employment for more than 600,000 people and up to 2 million people indirectly, generated approximately $2.4 billion in 2018 according to government statistics. Tanzania received a record 1.1 million international visitor arrivals in 2014, mostly from Europe, the US and Africa.

Tanzania is the only country in the world which has allocated more than 25% of its total area for wildlife, national parks, and protected areas.There are 16 national parks in Tanzania, 28 game reserves, 44 game-controlled areas, two marine parks and one conservation area.

Tanzania’s tourist attractions include the Serengeti plains, which hosts the largest terrestrial mammal migration in the world; the Ngorongoro Crater, the world’s largest intact volcanic caldera and home to the highest density of big game in Africa; Kilimanjaro, Africa’s highest mountain; and the Mafia Island marine park; among many others. The scenery, topography, rich culture and very friendly people provide for excellent cultural tourism, beach holidays, honeymooning, game hunting, historical and archaeological ventures – and certainly the best wildlife photography safaris in the world.

The objective of this project is to explore a sample dataset from Tanzania analyzing the tourism sector.

The challenge is sourced from [kaggle](https://www.kaggle.com/datasets/tevintemu/tanzania-tourism-classification-challenge) in case you want to find out more, visit the link.

## 1. <a name='TableofContents'></a>Table of Contents

<!-- vscode-markdown-toc -->

- 1. [Table of Contents](#TableofContents)
- 2. [Objectives, Planning and Folder Structure](#ObjectivesPlanningandFolderStructure)
  - 2.1. [Objectives](#Objectives)
  - 2.2. [Folder Structure](#FolderStructure)
- 3. [Setting up in your local environment](#Settingupinyourlocalenvironment)
  - 3.1. [Creating a virtual environment](#Creatingavirtualenvironment)
  - 3.2. [Activating your environment](#Activatingyourenvironment)
  - 3.3. [Deactivating your environment](#Deactivatingyourenvironment)
- 4. [Libraries and Installations](#LibrariesandInstallations)
  - 4.1. [Required Libraries](#RequiredLibraries)
  - 4.2. [Installation](#Installation)
- 5. [Starting your notebook](#Startingyournotebook)
- 6. [Disclaimer - use analysis with caution](#Disclaimer-useanalysiswithcaution)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

## 2. <a name='ObjectivesPlanningandFolderStructure'></a>Objectives, Planning and Folder Structure

### 2.1. <a name='Objectives'></a>Objectives

The [notebook](/tanzanian-analysis-eda.ipynb) does an exploratory data analysis on the data using a pandas DataFrame. The objectives of the project is to:

1. Load the dataset from csv's
2. Cleaning of the data - missing values, wrong values, duplicate values
3. A statistical summary on the numerical features
4. Analysis of the following questions:
   - Which are the top 3 countries that visitors come from?
   - What is the most common purpose of visitors by their age-group?
   - What is the data distribution of total costs based on country visitors are coming from, their age group and the purpose of their visit?
5. Visualization of the answered questions above

This repository is for beginner data analysts, data engineers and data scientists.

### 2.2. <a name='FolderStructure'></a>Folder Structure

The repository contains:

1. Datasets Directory - This directory holds our dataset - [Tanzania_Tourism_datasets.csv](/datasets/Tanzania_Tourism_datasets.csv, 'tanzania tourism dataset') The notebook contains the columns below:

- ID
- Country
- Age_group
- Travel_with
- Total_female
- Total_male
- Purpose
- Main_activity
- Info_source
- Tour_arrangement
<details>
<summary>Click to view other columns!</summary>
- Package_transport_int
- Package_accomodation
- Package_food
- Package_transport_tz
- Package_sightseeing
- Package_guided_tour
- Package_insurance
- Night_mainland
- Night_zanzibar
- Payment_mode
- First_trip_tz
- Most_impressing
- Total_cost
</details>

2. [Requirements.txt] (/requirements.txt) - Showing the necessary libraries and dependencies to run the notebook.
3. Notebooks
   - [tanzanian_analysis notebook](tanzanian-analysis-eda.ipynb)
4. [Gitignore File](/.gitignore) - File to ignore files and directories from being pushed to the remote repository
5. [README.md File](/README.md) - Guiding instructions for describing and running the project.

## 3. <a name='Settingupinyourlocalenvironment'></a>Setting up in your local environment

This section guides you on how to setup your environment and run the repository on your local environment.

### 3.1. <a name='Creatingavirtualenvironment'></a>Creating a virtual environment

Create a virtual environment to install and manage the libraries to isolate them from your global environments.

To create a virtual environment, run the command below on your terminal:

```bash
python -m venv 'myenv_name'
```

### 3.2. <a name='Activatingyourenvironment'></a>Activating your environment

To activate your environment on linux or mac operating system. Run the command below on your terminal.

```bash
source /path/to/myenv_name/bin/activate
```

To activate your environment on a windows environment:

```bash
source \path\to\myenv_name\Scripts\activate
```

### 3.3. <a name='Deactivatingyourenvironment'></a>Deactivating your environment

Once you're done working on the repository, REMEMBER to deactivate your virtual environment in order to separate your local project dependencies.

To deactivate your environment on a linux or mac operating system. Run the command below on your terminal:

```bash
deactivate
```

## 4. <a name='LibrariesandInstallations'></a>Libraries and Installations

### 4.1. <a name='RequiredLibraries'></a>Required Libraries

The important libraries used in this environment are:

1. Pandas - Used for manipulation, exploration, cleaning and analyzing of your dataset.
2. Numpy - Used for mathematical and statistical purposes often to prepare your dataset for machine learning
3. Matplotlib - Used for visualization purposes to highlight discovered patterns in your dataset to stakeholders in form of graphs
4. Seaborn - Used for visualization purposes to highlight discovered patterns in your dataset to stakeholders in form of graphs
5. Jupyter lab - Used to run and experiment on your notebook in your local environment

The above listed libraries are the core ones used in the repository. However, during installation you'll notice other dependencies installed that enable to work as expected. They are highlighted on the [requirement.txt](/requirements.txt) file.

### 4.2. <a name='Installation'></a>Installation

Ensure you are have a version python > 3 installed and running on your local environment in order to to be able to install the libraries and run the notebook. Afterwards, ensure the virtual environment you created above is active before running the installation commands below on your terminal.

To install the libraries run:

```bash
pip install pandas numpy matplotlib seaborn jupterlab
```

You can also install all the libraries by running:

```bash
pip install requirements.txt
```

## 5. <a name='Startingyournotebook'></a>Starting your notebook

To run your notebook in your local environment, we'll require the jupyter lab library installed. Afterwards, run the command below on your terminal:

```bash
jupyter lab *optional_file_name*
```

## 6. <a name='Disclaimer-useanalysiswithcaution'></a>Disclaimer - use analysis with caution ⚠️

1. The dataset is purely for learning purposes and hasn't been verified hence it isn't advisable to use it in a business setting as it might contain a wrong depiction of the tourism sector in Tanzania.
2. There are many ways to do the dataset wrangling other than the ones described in the (notebook)[data-science-projects//tanzanian-analysis-eda.ipynb].
