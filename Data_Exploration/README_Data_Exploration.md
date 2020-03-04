This Readme assume all steps of 'README_Data_Wrangling.md' completed successfully.

In order to replicate the Data Exploration portion of this project, please follow the following steps: 

1. Run the script "EEGVisualization.ipynb" in Google Colab. This script demonstrates that we could sucessfully read our raw data and display it using a speciality built package called NME.

2. Run the script "ChannelEnergy.ipynb" in Google Colab. Our initial attempt at understanding our data relied on the 2-norm to measure the "energy" of our EEGs. This script calculates 2-norm values for ALL waveforms in the data set. It then separates energy values by emotional label and electode, by creating multiple box-and-whisker plots. An important insight we learned in this step was that major energy outliers existed. In our next step, we determined where those outliers came from.

3. Run the script "2_NormOutlier.ipynb" in Google Colab. We wanted to determine where the 2-norm outlier values came from, so this script separated 2-norm values by patient id, again displaying the results as box-and-whisker plots. From this, we determined that a single electrode on patient 13 was the cause of outliers. We will remove these values during the modeling phase of the project.

4. Run the script "Wavelets.ipynb in Google Colab. This script attempted to quantify wavelet coefficients of individual waveforms. As the Wavelet Transform is a technique unfamiliar to most of the team, we did not uncover any significants insights from this script.

5. Run the script "EEGDiscreteCosineTransform.ipynb" in Google Colab. We next tried the Discrete Cosine transform, as it was a technique more familiar to the group. From the transforms of waveforms, we can see the cos coefficients that make up these signals. Our next step to this transform is to determine if correlation exists between the cos coefficients.

6. Run the scipt "Exploration.ipynb" in Google Colab. This script contains a variety of Data Exploration techniques, including PCA, Bar Charts, Correlation Heatplots, and FFTs. An important insight we noticed here was in the FFT files. While FFTs tend to have near-identical spectra, abnormal spikes within the 8-13Hz range occasionally appear. Our next step with the FFTs is to isolate this frequency range to see how distinct these spikes are.

7. This completes the Data Exploration phase of this project
