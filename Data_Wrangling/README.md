In order to replicate the Data Wrangling portion of this project, please follow the following steps:

1. Go to the Google Share Drive called: "DSCI400_Revamp". If you have proper authorization to view this project, an example "DSCI400_Revamp" shared drive will have already been shared with you.

2. Run the script "BDF_Full_Converter.ipynb" in Google Colab. This script will create two files called "Waveform_Data.h5" and "Label_Data.h5" within the drive, as well as two additional helper csv files. These files contained all the parsed waveform and label data of the "Sessions" folder condensed into two easy to access files.

3. Run the script "Phase_Vocoder.ipynb" in Google Colab. This script equalizes the length of all sessions' waveforms, as the waveforms recorded to different lengths. This script will create two files called "Waveform_Vocoded_Unequalized_Data.h5" and "Waveform_Vocoded_Equalized_Data.h5". The "Waveform_Vocoded_Equalized_Data.h5" contains all equal length waveforms

4. This completes the Data Wrangling/Preprocessing phase of this project. Proceed to the Data Exploration folder to continue...
