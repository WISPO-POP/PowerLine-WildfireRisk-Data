# PowerLine-WildfireRisk-Data
Data files of the wildfire risk associated with power lines, created by Sofia Taylor and Line A. Roald.

## Description
This repository contains CSV files of the wildfire ignition risk associated with power lines. The risk values are obtained by overlaying a map of electric power lines with historical wildfire risk maps, namely the Wind-enhanced Fire Potential Index (WFPI) maps from the U.S. Geological Survey. The WFPI maps are published once daily, and they indicate large fire and fire spread potential across the contiguous U.S. based on satellite imagery, fuel models, and weather forecasts.

Two systems of power lines are included. The first is the RTS-GMLC synthetic grid. The second is the actual transmission grid in California, which is publicly available through the California Energy Commission. The CSV data files in this repository contain risk values both for the full lines in these systems and for 10-km and 1-km line segments.

Since any particular line or line segment may intersect multiple levels of wildfire ignition risk, there are multiple ways to define the risk of that line or line segment. Here, two metrics of defining risk are included. First, the maximum risk metric defines the risk of a line segment as the maximum WFPI value that intersects that line segment. The cumulative risk metric defines the risk of a line segment as the integral of all of the intersecting risk values with respect to the line length. For more detailed information about how the risk values were assigned to the power lines in these systems, please see the publication listed below.

In total, there are 6 CSV data files in this repository. The file names follow the format: 
  grid_metric_segmentLength_startDate_endDate.csv

# Publication
If you would like to use this data, we kindly ask that you cite our publication:

  *Reference will be added soon.*

## Abstract
As wildfires in the United States are becoming more frequent and severe, mitigating wildfire ignition risk from power line faults is an increasingly crucial effort. Long-term ignition prevention strategies, especially converting overhead lines to underground cables, are expensive. Thus, it is important to prioritize upgrades on lines that will reduce wildfire ignition risk the most. However, since so many factors contribute to ignition risk, it is difficult to quantify the wildfire risk associated with power lines. This paper examines how various risk definitions based on historical wildfire risk maps can be used to inform transmission upgrade planning. These risk metrics are evaluated using an optimization model that determines which overhead lines should be undergrounded such that the total wildfire risk in the network is minimized. The risk assignment and upgrade selection are tested on both a synthetic network and the actual transmission lines in California.
