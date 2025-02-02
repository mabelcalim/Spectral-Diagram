# Spectral-Diagram (SD)

This repo refers to this article:

    Calim Costa et al., 2021: The Spectral Diagram as a new tool for model assessment in the frequency domain: Application to a global ocean general circulation model with tides, Computers and Geosciences, 2021,104977,ISSN 0098-3004,

  [CAGEO](https://doi.org/10.1016/j.cageo.2021.104977)
  [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0098300421002612)

 The Spectral Diagram (SD) is a new tool for the comparison of time series in the frequency domain. The SD provides a novel way to display the coherence function, power, amplitude, phase, and skill score of discrete frequencies of two time series. Each SD summarises these quantities in a single plot for multiple targeted frequencies.

Although the SD has been designed for tidal analysis, it is a powerful tool for detecting co-oscillating patterns in multi-scale analyses, and this approach might provide guidance in devising skill scores for inter-comparing model results.

Amplitude features in SDs:
    ![ScreenShot](https://github.com/mabelcalim/Spectral-Diagram/blob/main/figs/amp_explain.png)

Phase features in SDs:
    ![ScreenShot](https://github.com/mabelcalim/Spectral-Diagram/blob/main/figs/phase_explain.png)

# The following is a summary of appropriate and inappropriate uses of SDs:
  * Careful interpretation is required when a non-stationary time series is subjected to SD analysis. In such cases, localized transforms, e.g., wavelets, are preferable.
  * Ensures that the Nyquist frequency is not violated before using SD diagram. Such a violation can result in poor approximation of the chosen frequency (or band of frequencies) via SD analysis if the time series is too short or the sampling rate is not small enough.
  * The SD enables a multiple band of frequencies analysis without using filtering techniques, which implies convolution costs.
  * It is possible to track different time slots and multi-region comparisons using a normalized standard deviation of power strategy, with the drawback that  time series amplitude have to be scaled
  * It is a powerful tool to detect co-oscillating patterns in a multi scale analysis and anomalous patterns in a phenomena analysis.
  * SDs clearly display changes in amplitude and phase, thereby highlighting the co-oscillating frequencies to overcome the limited information contained in power spectrum analyses.
  * The need for better representing the degree of correspondence between simulated and observed fields for a given frequency (or frequency bands) is fulfilled by this novel tool inspired by relevant tide features.

Manual installation
-------------------
First steps:

    cd  PATH_TO_SAVE_SD_IN_YOUR_HOME
    git clone https://github.com/mabelcalim/Spectral-Diagram.git
    cd Spectral-Diagram/

    A local install can be done using the provided setup.py file:

        python3 setup.py install

    Pypi download
        python3 -m pip install SpecDiag==0.1.0

Support Group
==============

[users support group](https://groups.google.com/g/spectral-diagram)


Funding
==============
 This work was supported by National Counsel of Technological and Scientific Development (CNPQ), Grants No. 2012/02675-21, Coordination for the Improvement of Higher Education Personnel (CAPES) Grant No. 99999.005769/2014-00 (Migrado - BEX) (Doutorado-Sanduiche Australia), Bolsa Projeto CAPES/ANA BESM Grant No. 88887.115872/2015-01, and the National Institute for Science and Technology for Climate Change – INCT-MC Grant No. 465501/2014-1.
