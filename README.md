# Links to Practical Videos

*Practical #1: How to install the Ubuntu subsystem for Windows 10*  https://www.youtube.com/watch?v=22VtIhzPB1o

*Practical #2: Plotting data with Python and xmgrace*  https://www.youtube.com/watch?v=KrcyFavMHiY

*Practical #3: Detector Efficiency and Peak Fitting*  https://www.youtube.com/watch?v=OG-s4FhOMIk

*Practical #4: Semi-Empirical Mass Formula* https://www.youtube.com/watch?v=B2W0OYhtddY

# Introduction to Detector Efficiency and Peak Fitting
Introduction slides are included in this repository.

To download all the files included in this repository, paste in your terminal:

    git clone https://github.com/UWCNuclear/PeakFitting.git

# Doing the Efficiency Calibration of Real High Purity Germanium Detector Arrays!
Four data files are included in this repository:

*GRIFFIN* array at TRIUMF, Vancouver, Canada (16 germanium clover detectors): https://doi.org/10.1016/j.nima.2018.11.115

*MINIBALL* array at CERN, Geneva, Switzerland (8 germanium triple cluster detectors): https://doi.org/10.1140/epja/i2013-13040-9

*Soccer Ball* array at iThemba LABS, Cape Town, South Africa (13 germanium clover detectors): https://doi.org/10.1016/j.nima.2005.11.067

*TIGRESS* array at TRIUMF, Vancouver, Canada (12 germanium clover detectors): https://doi.org/10.1007/s10751-013-0905-7

# How to Find Nuclear Information 
*Lund/LBNL Nuclear Data Search:* http://nucleardata.nuclear.lu.se/toi/

*National Nuclear Data Center:* https://www.nndc.bnl.gov/


# How to Fit Peaks with GRSISort
*Installation instructions for Ubuntu and GRSISort at* https://github.com/UWCNuclear/UbuntuSetUp

(Remember Xming has to be run every time your computer is rebooted.)

Open the file with the following command, where ARRAYNAME is the name of the array with which you want to work:

    grsisort -l Eu152_ARRAYNAME.root

See the list of histograms in the file with ".ls"

Draw histogram with:

    gammaSingles->Draw()

Display rough peak energies by pressing "s"

Click and drag on x-axis to zoom in, zoom out by pressing "o", right click on x-axis and click “Unzoom” to zoom out

Click and drag on y-axis to zoom in, zoom out by pressing "o", right click on y-axis and click “Unzoom” to zoom out

Click on the left and click on the right side of the peak to set the fitting boundaries

Fit by pressing "f"

Remove all markers by pressing "n"

".q" to quit

***More analysis tools at*** https://github.com/GRIFFINCollaboration/GRSISort/wiki/Interactive-Analysis

# How to Fit the Detector Efficiency with RootEffi 
*Instructions and script at* https://github.com/UWCNuclear/RootEffi and in the introduction slides in this repo :-)

# PHY 312 Practicals

In one file, submit your fitted peaks (minimum of 8 peaks), your edited RootEffi script, and your efficiency curve :-)
