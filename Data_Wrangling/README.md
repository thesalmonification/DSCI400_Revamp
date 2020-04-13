# Data Wrangling Instructions
In order to replicate the Data Wrangling portion of this project, please follow the following steps:

1. Go to the Google Share Drive called: "DSCI400_Revamp". If you have proper authorization to view this project, an example "DSCI400_Revamp" shared drive will have already been shared with you.

2. Run the script `DataWranglingMasterScript.ipynb`. This script organizes all subscripts used to wrangle the data.

3. This completes the Data Wrangling/Preprocessing phase of this project. Proceed to the [Data Exploration Folder](https://github.com/thesalmonification/DSCI400_Revamp/tree/master/Data_Exploration/) and it's accompanying [README.md](https://github.com/thesalmonification/DSCI400_Revamp/tree/master/Data_Exploration/README.md) to continue...

### Interesting Data Wrangling Techniques Our Team Used

* Phase Vocoding: This technique, unlike simple up/downsampling, uses phase information to shorten signals which destroying spectra. We used this technique to shorten our EEG signals to equal length.

* Downsampling: After phase vocoding, we further shortened our EEG signals to reduce modeling complexity. To do so, we employed simple downsampling. Our signals were oversampled by a factor of 4.
