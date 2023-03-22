# Western Alps

The Western Alps database of onset times for earthquakes from 1989 to 2021 is composed of three files

## Station file: fsta_total.asc
============

The first line is the number of stations (only the first value is important)
We have 1043 stations with picks over an available list of 2064 stations.

Each line is composed of

ID_station
lon
lat
depth (in meter)
label (5 letters)
number of P picks
number of S picks

## Event file: fsrc_total.asc
==========

The first line is the total number of events and then the number of quakes. Blasts and shots are ignored in this database.

Each line is composed of

ID_event
lon
lat
depth (in km)  (as used by HYPO71)
origin time (should be zero at the beginning of the inversion)
unix time (en sec starting the 1sr January 1970)
date (yyyy.mm.dd-hh:mn:sec.msec)
label P
number of P picks
label S
number of S picks


## Picks file: fobs_total.asc

The first iine gives the total number of picks, the number of P picks and the number of S picks. (S picks follow P picks)

Each line is composed of 

ID_data
picked time (in sec)
picked uncertainty (in sec)
ID_event
ID_station
ID_ray (not defined)
number of P picks          (what follows are extra information)
number of S picks
total number of picks
pick label (P or S)
station label (in relation with the station ID)

This database is a fusion of different data collected from seismological agencies (see related paper for a better description)

Title
Assessing the reliability of local earthquake tomography for crustal imaging: 30 years of records in the Western Alps as a case study

Authors
J. Virieux, A. Paul, M. Langlais, A. Helmstetter, G. Janex, Philippe Guéguen, and L. Stehly

submitted to Geophysical Journal International




