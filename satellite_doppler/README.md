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

Linux User have to run dos2unix on the .tle file before using it!

## Flow graphs for gnuradio-companion:

* sat_doppler_corr_example.grc
  * Two methods implemented in embedded python blocks:
    * Method 1 predicts doppler frequency and uses external
      multiplication to correct doppler shift
    * Method 2 corrects doppler shift internally by using phase rotator

![Doppler frequency correction](sat_doppler_corr_example.png?raw=true "Doppler frequency correction")

## Installation:

The two described blocks are gnuradio embedded python blocks. You can copy from the example flow graph and paste them into your projects.
