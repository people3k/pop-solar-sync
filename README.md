# pop-solar-sync
Instructions to replicate work flow and analysis for Freeman et al.
2018, PNAS, “The synchronization of energy consumption by
human societies throughout the Holocene”
Freeman et al. 2018 PNAS

To replicate the workflow and analysis for Freeman et al 2018, PNAS “The synchronization of
energy consumption by human societies throughout the Holocene”, please follow the steps below.
One can either start with step one, or start with step two. If you begin with step two, you will
forgo downloading and cleaning all of the raw radiocarbon data. Once you reach step two, you
will use four directories: EnergyConsumption, RawDates, Simulated, SummaryAnalysis. The four
directories are housed in the FinalDataScripts.zip file. Download this file and follow the steps
below.

1. Download and and clean all of the raw data. The procedures for doing this can be found in
Freeman et al 2018, PNAS “The synchronization of energy consumption by human societies
throughout the Holocene” and in the RawDates directory for radiocarbon records. Once you
have downloaded and cleaned all of the raw data, you will need to calibrate the radiocarbon dates. Instructions for calibrating are in the RawDates directory, ReadmeCleanCalibrate.pdf. Once the radiocarbon data are cleaned and calibrated, construct the files in the EnergyConsumption directory in the Calib and Calib2 directories. This means summing the summed probability distributions over bins of 10-1000 years. You will also need to sum the raw radiocarbon ages into the same bins by age frequency. Note, the historical energy consumption data are annual resolution and not summed. The data sources for these historical data are in
Freeman et al 2018, PNAS “The synchronization of energy consumption by human societies
throughout the Holocene.”

2. Once the main files are constructed from step 1 (already constructed in the EnergyConsumption directory), access the EnergyConsumption directory and read the Readme.pdf file.Access the python scripts and CorrelationsandMI_R.pdf files to replicate the analysis of mutual information and Spearman’s correlations. Note, when using the python scripts, you will need to adjust your directories. If you run an R-script from within the energy consumption
directory, then the directory paths in CorrelationsandMI_R.pdf are all set correctly. These scripts will provide outputs that replicate Fig. 1 A-D in the Freeman et al. 2018, PNAS, as well as some figures in the supporting information. Once you have run the mutual information and correlations, you will need to construct summary files similar to those in the SummaryAnalysis directory. Read the Readme.tex file in SummaryAnalysis directory to understand the variables. In short, these files summarize all of the pairwise values of mutual information
and Spearman’s correlations in each particular data set.

3. Access the SummaryAnalysis directory and read the SummaryPlots.pdf file. Use the R-code
to replicate the plots, including Fig 1E and Fig. 2 in Freeman eta la. 2018, PNAS main
document.

4. Access the Simulated directory and use the R-script to simulate radiocarbon ages. Follow
the directions in the script to calibrate the ages for different standard errors and analyze the
raw and calibrated simulated dates. This will allow one to assess the effects of calibration on
synchrony. See the supporting information from Freeman et al. 2018, PNAS for more details.
