# Links to Practical Videos

*Practical #1: How to install the Ubuntu subsystem for Windows 10*  https://www.youtube.com/watch?v=22VtIhzPB1o

*Practical #2: Plotting data with Python and xmgrace*  https://www.youtube.com/watch?v=KrcyFavMHiY

*Practical #3: Detector Efficiency and Peak Fitting*  https://www.youtube.com/watch?v=OG-s4FhOMIk

*Practical #4: Semi-Empirical Mass Formula* https://www.youtube.com/watch?v=B2W0OYhtddY

# Introduction to Detector Efficiency and Peak Fitting
Introduction slides are included in this repository.

To download all the files included in this repository, paste in your terminal:

    git clone https://github.com/UWCNuclear/PeakFitting.git

# How to Fit Peaks with GRSISort
*Installation instructions for Ubuntu and GRSISort at* https://github.com/UWCNuclear/UbuntuSetUp

(Remember Xming has to be run every time your computer is rebooted :-)

From the PeakFitting directory (cd PeakFitting), open the file with the following command, where ARRAYNAME is the name of the array with which you want to work:

    grsisort -l Eu152_ARRAYNAME.root

See the list of histograms in the file with ".ls"

Draw histogram with:

    gammaSingles->Draw()

Display rough peak energies by pressing "s"

Click and drag on x-axis to zoom in, zoom out by pressing "o"

Click and drag on y-axis to zoom in, zoom out by pressing "o" or right click on y-axis and click “Unzoom”

Click on the left and click on the right side of the peak to set the fitting boundaries

Fit by pressing "f"

Remove all markers by pressing "n"

".q" to quit

***More analysis tools at*** https://github.com/GRIFFINCollaboration/GRSISort/wiki/Interactive-Analysis

# How to Do a Detector Efficiency Calibration with RootEffi 
The instructions and script are * https://github.com/UWCNuclear/RootEffi and in the introduction slides in this repository.

# PHY 312 Practicals
In one file, submit screenshots of your fitted peaks (minimum of 8 peaks), your edited RootEffi script, and your efficiency curve :-)


# More Details on Real High Purity Germanium Detector Arrays!
Four data files are included in this repository:

*GRIFFIN* array at TRIUMF, Vancouver, Canada (16 germanium clover detectors): https://doi.org/10.1016/j.nima.2018.11.115

*MINIBALL* array at CERN, Geneva, Switzerland (8 germanium triple cluster detectors): https://doi.org/10.1140/epja/i2013-13040-9

*Soccer Ball* array at iThemba LABS, Cape Town, South Africa (13 germanium clover detectors): https://doi.org/10.1016/j.nima.2005.11.067

*TIGRESS* array at TRIUMF, Vancouver, Canada (14 germanium clover detectors): https://doi.org/10.1007/s10751-013-0905-7

# How to Find Nuclear Information 
*Lund/LBNL Nuclear Data Search:* http://nucleardata.nuclear.lu.se/toi/

*National Nuclear Data Center:* https://www.nndc.bnl.gov/
