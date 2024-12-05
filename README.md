# DSC180A-Q1Project

## Project Overview

Wire routing congestion represents a significant challenge in contemporary chip design,
where the dense placement of interconnecting wires can lead to numerous complications.
These complications not only affect the overall performance of the chip but also contribute to
increased manufacturing costs. For instance, congestion can necessitate longer wire routes,
resulting in larger chip sizes and potentially introducing timing errors that compromise
functionality. As the demand for smaller chip sizes continues to grow and the cost of chip
development escalates, addressing congestion issues becomes increasingly critical.
Optimizing both component placement and routing within the chip design process offers a
potential pathway to mitigate congestion. Advances in machine learning present promising
opportunities in this regard. Specifically, machine learning tools can be leveraged to predict
congestion-prone areas or to suggest optimal placements and routing strategies to alleviate
congestion.

This project seeks to build a foundational understanding of the principles of chip design
and the application of graph machine learning techniques to this domain. The objective is
to explore how graph machine learning approaches can be utilized to model the domain
of chip design, aiming to predict and resolve congestion issues effectively. This will be
accomplished in two main steps. First, by completing exploratory data analysis on graph
data to build a base understanding of graph ml fundamentals. Next, by re-implementing
the paper DE-HNN (Luo et al., 2024).

## File Structure
* data - stores all datasets
* images - stores images from EDA
* src
  * ```DSC180-A1.ipynb``` - EDA for learning graph representation and basic congestion analysis.
  * ```EDA.ipynb``` - EDA for chips data
  * ```create_features.ipynb``` - creates the feature files to be used in the model training, validation, and testing
  * ```partition.ipynb``` - creates the partitions to be used in constructing virtual nodes as part of our model's architecture
  * ```processed_data_exploration.ipynb``` - exploring the structure of the processed chips data
  * ```train_xbar.ipynb``` - trains and validates DE-HNN model on XBAR data
* ```requirements.txt``` - requirements to run all files

## MTA Data: Accessing and Storing Data

Station Data has been provided in the data folder.

Station Data - [link](https://github.com/animeshbchowdhury/mta_subway_station/tree/main)

Ridership Data must be downloaded and added to the data folder alongside the provided station data.

Ridership/Trip Estimates Data - [link](https://drive.google.com/drive/folders/1fV47SWGv5_AFPR_gRfvK1ra1LfSFCgOw)

## Chips Data: Accessing and Storing Data

Processed Data (2023-03-06_data) - [link](https://zenodo.org/records/10795280?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6Ijk5NjM2MzZiLTg0ZmUtNDI2My04OTQ3LTljMjA5ZjA3N2Y1OSIsImRhdGEiOnt9LCJyYW5kb20iOiJlYzFmMGJlZTU3MzE1OWMzOTU2MWZkYTE3MzY5ZjRjOCJ9.WifQFExjW1CAW0ahf3e5Qr0OV9c2cw9_RUbOXUsvRbnKlkApNZwVCL_VPRJvAve0MJDC0DDOSx_RLiTvBimr0w)

Processed data must be downloaded from the link above, this data is used in ```EDA.ipynb``` and ```processed_data_exploration.ipynb```

Raw Data (NCSU-DigIC-GraphData-2023-07-25) - [link](https://drive.google.com/file/d/1Scq35gvCQvIMrmthGs7MUhc8c1VZ8ZwN/view)

Raw data must be downloaded from the link above, this data is used in ```create_features.ipynb```, ```partition.ipynb```, and ```train_xbar.ipynb``` by extension.

Ensure that you store all data under the data directory.

## Data Folder Structure:

Ensure that after downloading your data folder has this structure:

* data
  * 2023-03-06_data
  * chips
    * NCSU-DigIC-GraphData-2023-07-25
  * ```MTA_Subway_Origin-Destination_Ridership_Estimate__2024_20241008.csv```
  * ```MTA_Subway_Stations_updated.csv```

## How to Run Locally / Reproduce Results

### Setup
After pulling all provided code download and store the data as describe above. 

In a new virtual environment run ```pip install -r /path/to/requirements.txt```.

After setting up the virtual environment with the requirements, run ```create_features.ipynb``` and ```partition.ipynb```. These notebooks process our data and create files that will be used in other notebooks as described above.

### Part 1: MTA EDA
Run the Jupyter Notebook ```DSC180-A1.ipynb``` to reproduce results.

### Part 2: Chips Data
Run ```EDA.ipynb``` and ```processed_data_exploration.ipynb``` to see EDA for the chips data.

Run ```train_xbar.ipynb``` to see DE-HNN model training and validation
