# Links to Practical Videos

*Practical #1: How to install the Ubuntu subsystem for Windows 10*  https://www.youtube.com/watch?v=22VtIhzPB1o

*Practical #2: Plotting data with Python and xmgrace*  https://www.youtube.com/watch?v=KrcyFavMHiY

*Practical #3: Detector Efficiency and Peak Fitting*  https://www.youtube.com/watch?v=OG-s4FhOMIk

*Practical #4: Semi-Empirical Mass Formula* https://www.youtube.com/watch?v=B2W0OYhtddY

# Introduction to Semiconductors, Detector Efficiency and Peak Fitting
Introduction slides are included in this repository.

To download all the files included in this repository, paste in your terminal:

    git clone https://github.com/UWCNuclear/DetectorEfficiency.git

# How to do a Detector Efficiency Calibration

For this practical, Ubuntu/Linux, ROOT and GRSISort are required.

*Installation instructions:* https://github.com/UWCNuclear/UbuntuSetUp

(Remember Xming has to be run every time your computer is rebooted :-)

Download the .root data files and slides with

    git clone https://github.com/UWCNuclear/DetectorEfficiency.git

Download the RootEffi efficiency script with

    git clone https://github.com/UWCNuclear/RootEffi.git

Move the RootEffi script to the DetectorEfficiency directory:

    cd DetectorEfficiency
    mv ../RootEffi.C .

In gedit, open the RootEffi.C script to see the energy of the peaks you should fit:

    gedit RootEffi.C &

In GRSISort, open the data file of your choice, where ARRAYNAME is the name of the array with which you want to work (GRIFFIN, MINIBALL, SoccerBall or TIGRESS):

    grsisort -l Eu152_ARRAYNAME.root

Fit the peaks of interest (tips in the section below!), and save screenshots of your fitted peaks and their fitted area/sum (minimum of 8 peaks)

In the RootEffi.C script, edit the peak areas and uncertainties obtained from the peaks you fitted.

Remember that whenever you edit a script, you should save it and close ROOT/GRSISort to run it again.

To run RootEffi, type in the command line:

    grsisort -l RootEffi.C

Save your edited script and your new efficiency curve

In one file, submit screenshots of your fitted peaks (minimum of 8 peaks), your edited RootEffi script, and your efficiency curve :-)

# How to Fit Peaks with GRSISort

From the DetectorEfficiency directory (cd DetectorEfficiency), open the file with the following command, where ARRAYNAME is the name of the array with which you want to work:

    grsisort -l Eu152_ARRAYNAME.root

See the list of histograms in the file with ".ls"

Draw histogram with:

    gammaSingles->Draw()

Display rough peak energies by pressing "s"

Click and drag on the x-axis to zoom in, zoom out by pressing "o"

Click and drag on the y-axis to zoom in, zoom out by pressing "o" or right click on the y-axis and click “Unzoom”

Click on the left and click on the right side of the peak to set the fitting boundaries

Fit by pressing "f"

Remove all markers by pressing "n"

".q" to quit

***More analysis tools at*** https://github.com/GRIFFINCollaboration/GRSISort/wiki/Interactive-Analysis

# More Details on Real High Purity Germanium Detector Arrays!
Four data files are included in this repository:

*GRIFFIN* array at TRIUMF, Vancouver, Canada (16 germanium clover detectors): https://doi.org/10.1016/j.nima.2018.11.115

*MINIBALL* array at CERN, Geneva, Switzerland (8 germanium triple cluster detectors): https://doi.org/10.1140/epja/i2013-13040-9

*Soccer Ball* array at iThemba LABS, Cape Town, South Africa (13 germanium clover detectors): https://doi.org/10.1016/j.nima.2005.11.067

*TIGRESS* array at TRIUMF, Vancouver, Canada (14 germanium clover detectors): https://doi.org/10.1007/s10751-013-0905-7

# How to Find Nuclear Information 
*Lund/LBNL Nuclear Data Search:* http://nucleardata.nuclear.lu.se/toi/

*National Nuclear Data Center:* https://www.nndc.bnl.gov/
