# Introduction on Detector Efficiency and Peak Fitting
Introduction slides are included in this repository.

To download all the files included this repository, paste in your terminal:

    git clone https://github.com/UWCNuclear/PeakFitting.git

# Doing the Efficiency Calibration of Real Germanium Detector Arrays!
Four data files are included in this repository:

*GRIFFIN* array at TRIUMF, Vancouver, Canada (16 germanium clover detectors, 16 x 4 = 64 germanium crystals)

*MINIBALL* array at CERN, Geneva, Switzerland (8 germanium triple cluster detectors, 8 x 3 = 24 germanium crystals)

*Soccer Ball* array at iThemba LABS, Cape Town, South Africa (13 germanium clover detectors, 13 x 4 = 52 germanium crystals)

*TIGRESS* array at TRIUMF, Vancouver, Canada (12 germanium clover detectors, 12 x 4 = 48 germanium crystals)

# How to Find Nuclear Information 
*The Lund/LBNL Nuclear Data Search:* http://nucleardata.nuclear.lu.se/toi/

*National Nuclear Data Center:* https://www.nndc.bnl.gov/

# How to Fit Peaks with GRSISort
*Installation instructions for Ubuntu and GRSISort at* https://github.com/UWCNuclear/UbuntuSetUp

Open the file with “ grsisort -l Eu152_ARRAYNAME.root ”

See the list of histograms in the file with “.ls”

Draw histogram with “ gammaSingles->Draw() ”

Display peak energies by pressing “s”

Click and drag on x-axis to zoom in, zoom out by pressing “o”

Click and drag on y-axis to zoom in, right click and click “Unzoom” to zoom out

Click and click on spectrum to set the fitting boundaries around your peak

Fit by pressing “f”

Remove all markers by pressing “n”

.q to quit

***More analysis tools at*** https://github.com/GRIFFINCollaboration/GRSISort/wiki/Interactive-Analysis

# How to Fit the Detector Efficiency with RootEffi 
https://github.com/UWCNuclear/RootEffi

Instructions are on the GitHub page and in the README file, and in the Introduction slides :-)

