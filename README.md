##### The suite of code given here are for classifying audio signal from the free spoken digit dataset ([FSDD](https://github.com/Jakobovski/free-spoken-digit-dataset)) using random forest classifier algorithm.
---
##### This work is posted on [Medium](https://medium.com/@neelakshij/6ab4df23e072)
***
##### Contents:

- __objective__
- __data__
- __required libraries__
- __analysis__
- __summary__
- __Acknowledgements__

**Objective**
: classifying audio signal from the free spoken digit dataset (FSDD) using random forest classifier algorithm.

**Data**
: The FSDD is an open dataset. It contains spoken digits 0 to 9 in English, with 50 repetitions recorded by 6 different male speakers with neutral, French, German, and Greek accents. Audios are in the wav format with 8 kHz sampling rate.

**Required libraries** 
- Librosa 
- Sklearn
- NumPy 
- SciPy 
- Pandas 

**Analysis** 
- Preprocessing:
    explore_data.ipynb file checks for the type of the audio (mono or stereo) and sampling rate. 
* Extract features: 
    MFCCs and their first and second order derivatives are extracted using librosa package. Statistical measures are computed using numpy and scipy libraries. 
+ Classification: 
    Random Forest classifier is used. Obtained 97% accuracy with 10-fold cross-validation.

**Summary** 
: To summarize, a standardized audio dataset FSDD is used to demonstrate the accuracy in classifying audio signals using Random Forest classifier. Preprocessing audio signal is performed followed by extracting features using librosa. Random forest classifier used from sklearn library.

**Acknowledgements**
* Zohar Jackson, César Souza, Jason Flaks, Yuxin Pan, Hereman Nicolas, & Adhish Thite. (2018, August 9). Jakobovski/free-spoken-digit-dataset: v1.0.8 (Version v1.0.8). Zenodo. http://doi.org/10.5281/zenodo.1342401
* McFee, Brian, Colin Raffel, Dawen Liang, Daniel PW Ellis, Matt McVicar, Eric Battenberg, and Oriol Nieto. “librosa: Audio and music signal analysis in python.” In Proceedings of the 14th python in science conference, pp. 18-25. 2015.
* Scikit-learn: Machine Learning in Python, Pedregosa et al., JMLR 12, pp. 2825-2830, 2011.
* Harris, C.R., Millman, K.J., van der Walt, S.J. et al. Array programming with NumPy. Nature 585, 357–362 (2020). DOI: 0.1038/s41586-020-2649-2.
* SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.
* Pandas-dev/pandas: Pandas, DOI: 10.5281/zenodo.3509134.
