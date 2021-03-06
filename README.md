# Belly Button Biodiversity

![Bacteria by filterforge.com](Images/bacteria.jpg)

This is an interactive dashboard to explore the [Belly Button Biodiversity dataset](http://robdunnlab.com/projects/belly-button-biodiversity/), which catalogs the microbes that colonize human navels.

The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.

## Overview

I used the D3 library to read in `samples.json` then created a horizontal bar chart with a dropdown menu to display the top 10 OTUs found in that individual.  Then used `sample_values` as the values for the bar chart.  Next I used `otu_ids` as the labels for the bar chart and `otu_labels` as the hovertext for the chart.

![bar Chart](Images/hw01.png)

Next I created a bubble chart that displays each sample.  Then I useD `otu_ids` for the x values, `sample_values` for the y values, `sample_values` for the marker size, `otu_ids` for the marker colors, and `otu_labels` for the text values.

![Bubble Chart](Images/bubble_chart.png)

I displayed the sample metadata, i.e., an individual's demographic information.  Then displayed each key-value pair from the metadata JSON object somewhere on the page.

![hw](Images/hw03.png)

I updated all of the plots any time that a new sample is selected.  

![hw](Images/hw02.png)

