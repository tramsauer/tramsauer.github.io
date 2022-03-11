layout: page
title: raddo
permalink: /raddo/

# [**raddo**:  RADOLAN Weather Radar Data Downloader](https://github.com/tramsauer/raddo)

[![license badge](https://img.shields.io/badge/license-GNU_GPLv3-blue)](LICENSE.txt)
[![Build Status: master](https://travis-ci.com/tramsauer/raddo.svg?branch=main)](https://app.travis-ci.com/github/tramsauer/raddo)
[![Docker Build Status](https://img.shields.io/docker/cloud/build/tramsauer/raddo?logo=docker)](https://hub.docker.com/r/tramsauer/raddo/)
[![GitHub release](https://img.shields.io/github/release/tramsauer/raddo.svg?logo=github)](https://github.com/tramsauer/raddo/releases/latest)
[![Documentation Status](https://readthedocs.org/projects/raddo/badge/?version=stable)](https://raddo.readthedocs.io/en/stable/?badge=stable)

*raddo* helps you find, download, sort and preprocess RADOLAN weather radar precipitation data for further usage.


*raddo* downloads and processes RADOLAN weather radar ASCII data.
Downloaded files are sorted in folders based on year and month and may also be decompressed.
As next step *raddo* creates GeoTiffs in generic WGS84 lat/lon coordinates and/or a single NetCDF file upon user request.
In case the data is only needed for a smaller region, masking via a shapefile is also possible.
For all possibilities on data retrieval and processing see the *usage section*.

*raddo* tries to download all recent RADOLAN ASCII files / archives from the DWD FTP server to the specified directory if files do not exist already. A list of dates possibly available is used to compare hypothetical available data sets with actual local available ones. So file listing on the FTP side is skipped due to (formerly) unreliable connection.

RADOLAN data from the German Weather Service (Deutscher Wetterdienst, DWD) is copyrighted! Please find the copyright text [here](https://opendata.dwd.de/climate_environment/CDC/Terms_of_use.pdf).
The freely accessible data may be re-used without any restrictions provided that the source reference is indicated, as laid down in the GeoNutzV ordinance.

The RADOLAN precipitation data files are *updated daily* by DWD.

<img align="right" src="https://github.com/tramsauer/raddo/blob/main/dwd_logo.png" width="200">

The data can be found at [opendata.dwd.de](https://opendata.dwd.de/climate_environment/CDC/grids_germany/hourly/radolan/recent/asc/ "https://opendata.dwd.de/climate_environment/CDC/grids_germany/hourly/radolan/recent/asc/").

