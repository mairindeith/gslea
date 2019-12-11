[![stability-wip](https://img.shields.io/badge/stability-work_in_progress-lightgrey.svg)](https://github.com/orangemug/stability-badges)

Gulf of St. Lawrence Ecosystem Approach package
===============================================

This package offers a database of measured variables which can inform an
ecosystem approach for the Gulf of St. Lawrence, Canada. In addition to
a dataset at the ecoregion level, standard query functions are provided
to extract relevant data series.

This package is intentionally kept small and aggregated to facilitate
analyses that call it without breaking existing analyses that depend on
it and to feed other analyses with only limited need to look at the guts
of this package. The package does not provide data at a sample by sample
level but always integrated to the ecoregion level. If you would like to
have finer scale data it is suggested that you first consult the
references in the dataset help files and then the individual responsble
for that data.

    devtools::install_github(https://github.com/duplisea/gslea)
    library(gslea)

State of development
--------------------

This database presently includes physical oceanographic and biological
oceanographic data for the Gulf Ecoregions.

Map of the Gulf of St Lawrence with Ecoregions and fish survey stations
-----------------------------------------------------------------------

Data available
--------------

Presently, gslea includes physical oceanographic, chemical
oceanographic, planktonic and phenological data. These data are stored
as a data.table called EA.data which is a long format table with one row
per observation and which enables an efficient data extraction that can
enable other analyses. Auxially datasets for mapping such as bathymetry
are also included and descriptive table describing the ecosystem
measured variables.

Extracting data
---------------

a scatterplot of all the different environmental variables
==========================================================

### Project particpants

Hugues Benoît, Daniel Duplisea, Peter Galbraith, David Merette, Stéphane
Plourde, Marie-Julie Roux, Bernard Sainte-Marie
