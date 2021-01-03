# Satellite Doppler Frequency Shift Correction

Correct satellite doppler frequency shift.


## Depends on: 

* python3-orbit-predictor


## Configuration:

Set sample_rate, receive frequency, receiver location (lat, lon, height,
name), TLE file with satellite data (must fit to data source - so don´t use
new .tle files together with older data records), satellite name in .tle
file (watch for disturbing trailing white spaces after name in tle), start
time of record (format '2021-01-02 08:09:15') and timezone for it
(e.g. 'Europe/Berlin').


## Installation:

Run hier block once in gnuradio-companion to install. After "Reload Blocks" or restart
of gnuradio-companion they will appear under "GRC Hier Blocks".


## Flow graphs for gnuradio-companion:

* sat_doppler_corr_hier.grc
  * Satellite Doppler Frequency Shift Correction

* sat_doppler_corr_example.grc
  * Example using Hier Block
