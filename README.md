# audio-digits-classification
The suite of code given here are for classifying audio signal from the free spoken digit dataset (FSDD) using random forest classifier algorithm.
link: https://github.com/Jakobovski/free-spoken-digit-dataset

This work is posted on Medium (https://medium.com/@neelakshij/6ab4df23e072)

Contents:
1. objective
2. data 
3. required packages
4. analysis
5. summary
6. Acknowledgements

Objective
classifying audio signal from the free spoken digit dataset (FSDD) using random forest classifier algorithm.

Data
The FSDD is an open dataset. It contains spoken digits 0 to 9 in English, with 50 repetitions recorded by 6 different male speakers with neutral, French, German, and Greek accents. Audios are in the wav format with 8 kHz sampling rate.

Required Packages
librosa
NumPy
SciPy
pandas
Sklearn

Analysis
a. Preprocessing:
   explore_data.ipynb file checks for the type of the audio (mono or stereo) and sampling rate.
b. extract features:
   MFCCs and their first and second order derivatives are extracted using librosa package. Statistical measures are computed using numpy and scipy libraries. 
c. classification:
   Random Forest classifier is used. Obtained 97% accuracy with 10-fold cross-validation.
   
   
Summary
To summarize, a standardized audio dataset FSDD is used to demonstrate the accuracy in classifying audio signals using Random Forest classifier. Preprocessing audio signal is performed followed by extracting features using librosa. Random forest classifier used from sklearn library.

Acknowledgements
1) Zohar Jackson, César Souza, Jason Flaks, Yuxin Pan, Hereman Nicolas, & Adhish Thite. (2018, August 9). Jakobovski/free-spoken-digit-dataset: v1.0.8 (Version v1.0.8). Zenodo. http://doi.org/10.5281/zenodo.1342401
2) McFee, Brian, Colin Raffel, Dawen Liang, Daniel PW Ellis, Matt McVicar, Eric Battenberg, and Oriol Nieto. “librosa: Audio and music signal analysis in python.” In Proceedings of the 14th python in science conference, pp. 18-25. 2015.
3) developers of NumPy, SciPy and Sklearn libraries.
