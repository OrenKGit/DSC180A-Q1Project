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

## Accessing and Storing Data

Station Data has been provided in the data folder.

Station Data - https://github.com/animeshbchowdhury/mta_subway_station/tree/main

Ridership Data must be downloaded and added to the data folder alongside the provided station data.

Ridership/Trip Estimates Data - https://drive.google.com/drive/folders/1fV47SWGv5_AFPR_gRfvK1ra1LfSFCgOw

## File Structure
* SRC
  * Notebooks
    * DSC180-A1.ipynb - EDA for learning graph representation and basic congestion analysis.
* Data
* requirements.txt

## How to Run Locally / Reproduce Results

After pulling all provided code download and store the data as describe above. 

In a new virtual environment run ```pip install -r /path/to/requirements.txt```.

Run the Jupyter Notebook ```DSC180-A1.ipynb``` to reproduce results.
