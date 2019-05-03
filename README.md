# EEG Visualization Shiny App
#### DS4BME Project Documentation

This App loads EEG data files that are in ".set" format and provide different plots based on user selection.  
#### Background:
In research of haptics and sensory feedback of neuroprostheses, it is important to understand the neural representation based on peripheral input
such as electrocutaneous, mechanotactile, or vibrotactile stimulations. Whether the differences of stimulation modalities and parameters will be captured
by non-invasive neural recordings is still under investigation. The neural signal used in the studies is electroencephalogram (EEG),
which has 64 electrodes. During an EEG recording, stimulation onset is known as an epoch. 
In the sample dataset, there are ten stimulation events (epochs).

#### Features of this app include:  
1. Display different epochs of EEG recording and allows user selection  
2. Based on epoch selection, plot EEG data with different colors representing electrodes
3. Bandpass filter based on user input frequency bands
4. Within the selected frequency band:  
  a. plot the spectrogram of the electrode with highest power  
  b. plot the topographical layout
5. Allow custom user file input and plot download as .png file

#### Specific instructions on file input:  
The imported data needs to be preprocessed EEG data, in ".set" format.  
With the nature of EEG data file complexity, the read-in of data requires both a .set and a .fdt files with the same filename,
under the same directory. The example custom data input of this app is taken from [my GitHub repo](https://github.com/KQDing/dsData).  
[sample custom data](https://raw.githubusercontent.com/KQDing/dsData/master/sample.set)  
