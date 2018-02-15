# pop-solar-sync
Meta data file for Freeman et al.: "Global synchrony of human populations and solar energy throughout the Holocene" 

The data consists of two folders. The first called "python" contains data and scrips for running a high frequency synchrony analysis of the radiocarbon data and solar energy data. The second folder called "R" contains data files and scripts for running low frequency correlation analysis of the radiocarbon and solar energy data.

Files: Each folder contains data files. The "python" folder contains five data files: calibdata_all.csv, calibdata200.csv, calibdata300.csv, rawdata_all.csv and rawdata300.csv. The file calibdata_all.csv contains the frequencies of median calibrated radiocarbon ages in 100, 200, and 300 year bins along with the frequency of sunspots. The file rawdata_all.csv contains uncalibrated radiocarbon ages for 5 western states binned at 100 and 300 year intervals. The other files are subsets of these two largerfiles noted by 200, 300, etc (i.e., only 300 year bins). The R folder contains three files: SyncData1.csv, SyncData2.csv and SyncData3.csv. These are files that bin calibrated radiocarbon ages and sunspot frequencies at 100, 200, and 300 year intervals respecively.

Scripts: The `"python" folder contains five python scrips, one for each bin size and calibration ID (yes or no) (100, calibrated; 200, calibrated, 300; calibratd; 100, raw dates; and 300, raw dates. Running the srcipts allows one to jconduct our high freequency correlation (phase locking analysis). The ``R" folder contains an R-script that allows one to replicate basic plots and low frequency correlations (Spearman's correlations for the entire 10,000 year interval). 

Data: The variables are consistently named across files. The only difference being whether ages are raw or calibrated, marked by each csv file.

bp--This variable indicates the begining bin value for all aggregated radiocarbon ages and sunspot frequencies.

sun--This variable is the estimated number of sunspots in a given bin of 100, 200, or 300 years. The data are from:
Sami K Solanki, Ilya G Usoskin, Bernd Kromer, Manfred Sch¸ssler, and J¸rg Beer. Unusual activity of the sun during recent decades compared to the previous 11,000 years. Nature, 431(7012):1084ñ1087, 2004.

ariz--the frequency of median radiocarbon ages from the state of Arizona in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

cali--the frequency of median radiocarbon ages from the state of California in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

colo--the frequency of median radiocarbon ages from the state of Colorado in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

nmex--the frequency of median radiocarbon ages from the state of New Mexico in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

neva--the frequency of median radiocarbon ages from the state of Nevada in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

utah--the frequency of median radiocarbon ages from the state of Utah in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

wyom--the frequency of median radiocarbon ages from the state of Wyoming in a given bin. Raw data from: CARD. CARD 2.0. http://www.canadianarchaeology.ca/, 2017

chile--the frequency of median radiocarbon ages from N. Chile Atacama desert in a given bin. Raw data from: Eugenia M Gayo, Claudio Latorre, and Calogero M Santoro. Timing of occupation and regional settlement patterns revealed by time-series analyses of an archaeological radiocarbon database for the South-Central Andes (16ñ25 s). Quaternary International, 356:4ñ14, 2015.

uk--the frequency of median radiocarbon ages from England, Scotland and Ierland in a given bin. Raw data from: Andrew Bevan. Radiocarbon Dataset and Analysis from Bevan, A., Colledge, S., Fuller, D., Fyfe, R., Shennan, S. and C. Stevens 2017. Holocene fluctuations in human population demonstrate repeated links to food production and climate. http://discovery.ucl.ac.uk/10025178/, 2017. Note, we have variables that denote the regions identified by Bevan et al., but do not use these in our analysis.

aus--the frequency of median radiocarbon ages from Australia in a given bin. Raw data from: Alan Williams and Sean Ulm. AustArch: A database of 14c and luminescence ages from
archaeological sites in Australia [data-set]. https://doi.org/10.5284/1027216, 2014.

usa--the summed frequency of median radiocarbon ages from all of the western US states noted above in a given bin. 
