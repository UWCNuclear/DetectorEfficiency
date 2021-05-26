# Introduction to Detector Efficiency and Peak Fitting
Introduction slides are included in this repository (soon!).

To download all the files included in this repository, paste in your terminal:

    git clone https://github.com/UWCNuclear/PeakFitting.git

# Doing the Efficiency Calibration of Real High Purity Germanium Detector Arrays!
Four data files are included in this repository:

*GRIFFIN* array at TRIUMF, Vancouver, Canada (16 germanium clover detectors, 16 x 4 = 64 germanium crystals): https://doi.org/10.1016/j.nima.2018.11.115

*MINIBALL* array at CERN, Geneva, Switzerland (8 germanium triple cluster detectors, 8 x 3 = 24 germanium crystals): https://doi.org/10.1140/epja/i2013-13040-9

*Soccer Ball* array at iThemba LABS, Cape Town, South Africa (13 germanium clover detectors, 13 x 4 = 52 germanium crystals): https://doi.org/10.1016/j.nima.2005.11.067

*TIGRESS* array at TRIUMF, Vancouver, Canada (12 germanium clover detectors, 12 x 4 = 48 germanium crystals): https://doi.org/10.1007/s10751-013-0905-7

# How to Find Nuclear Information 
*Lund/LBNL Nuclear Data Search:* http://nucleardata.nuclear.lu.se/toi/

*National Nuclear Data Center:* https://www.nndc.bnl.gov/


# How to Fit Peaks with GRSISort
*Installation instructions for Ubuntu and GRSISort at* https://github.com/UWCNuclear/UbuntuSetUp

Open the file with " grsisort -l Eu152_ARRAYNAME.root "

See the list of histograms in the file with ".ls"

Draw histogram with " gammaSingles->Draw() "

Display rough peak energies by pressing "s"

Click and drag on x-axis to zoom in, zoom out by pressing "o", right click on x-axis and click “Unzoom” to zoom out

Click and drag on y-axis to zoom in, zoom out by pressing "o", right click on y-axis and click “Unzoom” to zoom out

Click on the left and click on the right side of the peak to set the fitting boundaries

Fit by pressing "f"

Remove all markers by pressing "n"

".q" to quit

***More analysis tools at*** https://github.com/GRIFFINCollaboration/GRSISort/wiki/Interactive-Analysis

# How to Fit the Detector Efficiency with RootEffi 
*Instructions and script at* https://github.com/UWCNuclear/RootEffi

Instructions are on the GitHub page, its README file, and in the introduction slides :-)

