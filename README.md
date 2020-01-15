# asymmetric sampling
Giroud et al. PloS Biology 2020 "Asymmetric sampling in human auditory cortex reveals spectral processing hierarchy"


the folder contains the followings datasets: 
- individual_itpc_pure_tones_ROIs.npy 
it represents the individual itpc values for each subject arranged by ROIs.
it is of size : nb_subjects * nb_frequencies * nb_timesamples
(39, 200, 334) ROI 1 : left Primary Auditory cortex (lPAC)
(27, 200, 334) ROI 2 : right Primary Auditory cortex (rPAC)
(40, 200, 334) ROI 3 : left Secondary Auditory cortex (lSAC)
(29, 200, 334) ROI 4 : right Secondary Auditory cortex (rSAC)
(12, 200, 334) ROI 5 : left  Auditory Association cortex (lAAC)
(12, 200, 334) ROI 6 : right Auditory Association cortex (rAAC)

- frequencies.npy
it represents the frequencies in Hz used for calculating ITPCs
200 freqs between 2 HZ and 250Hz log spaced
python code : freqs= np.logspace(*np.log10([2, 250]), num=200)
