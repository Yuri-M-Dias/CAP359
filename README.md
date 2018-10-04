# CAP-359-3

This is a repository for the "Data Mining" discipline at INPE/CAP.

# Project idea

This project is being made by:

- Caio Gustavo Rodrigues da Cruz
- Yuri Matheus Dias Pereira

The idea is to use data mining techniques to extract information from satellite telemetry data, to aid with mission control operations.

More specifically, in this project we will apply *motif discovery* and *association rules mining* algorithms and techniques to satellite telemetry data, treating them as time series.
The aim with the motif discovery is to see patterns on the satellite subsystems that might signal a possible equipment degradation or anomalous behaviour, while the goal of the association rules mining is to see how the different subsystems telemetry readings impact on each others.

## Data

The available data consists of several months and years of one of INPE's operational satellites. It consists of 135 telemetries, read at every half a second during each satellite passage over one of the available ground stations.

## Algorithms, packages and implementation

For the motif discovery part, the [jmotif-R](https://github.com/jMotif/jmotif-R) package will be used, as it already implements the relevant [SAX](http://www.cs.ucr.edu/~eamonn/SAX.htm) algorithms and support algorithms.
Additionally, the [DTW technique](http://dtw.r-forge.r-project.org/) will be used to validate the found discords in relation to the rest of the time series.

**Needs the algorithms for the association rule mining part**

# Results and timeline

A report will be made with the results found and applied algorithms in the end of the discipline period, by the 10th of december, on this repository.

