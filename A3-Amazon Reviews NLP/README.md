# Generating Useful Features for Further Analysis on Amazon Reviews

## Introduction

### Business Context
Clients want to analyze reviews of their products on Amazon (as opposed to Yelp) to answer key strategic questions:
* What are the most important factors driving negative reviews?
* Have there been significant changes to customer satisfaction and reviews over time?

---

### Business Problem
The primary objective is to **explore the given data and use the results of the investigation to engineer relevant features** that will facilitate subsequent downstream analysis and predictive model-building.

---

### Analytical Context
The dataset contains a large collection of movie and television reviews submitted on Amazon between 1996 and 2014. 

A central challenge during text processing is that words often carry different meanings depending on context. For example, common words like `"good"` frequently appear across both positive and negative reviews. Appropriate natural language processing (NLP) and feature engineering techniques must be developed to interpret such words accurately.

---

## Loading the Data

The analysis utilizes subsets of data sourced from the [UCSD Amazon Review Dataset repository](http://jmcauley.ucsd.edu/data/amazon/):
* **Amazon Instant Video Reviews:** ~37,000 reviews
* **Movies and TV Reviews:** ~1,700,000 reviews

> **Note on Data Format:** The datasets are gzip-compressed (`.json.gz`) line-delimited JSON files, where each line represents a standalone review stored as an individual JSON object.

## Repository Notes & File Availability

Due to GitHub file size limitations, the raw data files are not hosted directly in this repository. 

To run or review the analysis:
* The original source datasets directly from the [UCSD Amazon Review Dataset repository](http://jmcauley.ucsd.edu/data/amazon/).
* The completed analysis, processed outputs, and final solutions are fully provided in the repository's answer file (`assignment_3_STUDENT.html`).
