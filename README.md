# Links to Practical Videos

*Practical #1: How to install the Ubuntu subsystem for Windows 10*  https://www.youtube.com/watch?v=22VtIhzPB1o

*Practical #2: Plotting data with Python and xmgrace*  https://www.youtube.com/watch?v=KrcyFavMHiY

*Practical #3: Detector Efficiency and Peak Fitting*  https://www.youtube.com/watch?v=OG-s4FhOMIk

*Practical #4: Semi-Empirical Mass Formula* https://www.youtube.com/watch?v=B2W0OYhtddY

# Introduction to Semiconductors, Detector Efficiency and Peak Fitting
Introduction slides are included in this repository along with four data files:

- *GAMKA* array at iThemba LABS, Cape Town, South Africa (13 germanium clover detectors): https://doi.org/10.1016/j.nima.2005.11.067

- *GRIFFIN* array at TRIUMF, Vancouver, Canada (16 germanium clover detectors): https://doi.org/10.1016/j.nima.2018.11.115

- *MINIBALL* array at CERN, Geneva, Switzerland (8 germanium triple cluster detectors): https://doi.org/10.1140/epja/i2013-13040-9

- *TIGRESS* array at TRIUMF, Vancouver, Canada (14 germanium clover detectors): https://doi.org/10.1007/s10751-013-0905-7

# How to Find Nuclear Information

- Lund/LBNL Nuclear Data Search: http://nucleardata.nuclear.lu.se/toi/

- National Nuclear Data Center: https://www.nndc.bnl.gov/

# How to do a Detector Efficiency Calibration

For this practical, Ubuntu/Linux, gedit, ROOT and GRSISort are required.

*Installation instructions:* https://github.com/UWCNuclear/UbuntuSetUp

(Remember Xming has to be run every time your computer is rebooted :-)

**Step 1.** Download the .root data files and slides by pasting the following command in your Ubuntu terminal and pressing Enter:

    git clone https://github.com/UWCNuclear/DetectorEfficiency.git

**Step 2.** Once the previous command it done, download the RootEffi efficiency script with the command:

    git clone https://github.com/UWCNuclear/RootEffi.git

**Step 3.** Move into the DetectorEfficiency directory with the command:

    cd DetectorEfficiency

and move the RootEffi script to the DetectorEfficiency directory with the command:
    
    mv ../RootEffi/RootEffi.C .

**Step 4.** Open the RootEffi.C script in gedit to see the energy of the peaks you should fit:

    gedit RootEffi.C &

**Step 5.** Open the data file of your choice in GRSISort with the following command, by changing ARRAYNAME to the name of the array with which you want to work (GAMKA, GRIFFIN, MINIBALL or TIGRESS):

    grsisort -l Eu152_ARRAYNAME.root

**Step 6.** See the list of histograms in the file by typing ".ls" in the GRSISort terminal. Draw the histogram by pasting the following command:

    gammaSingles->Draw()

**Step 7.** Fit a peak of interest to obtain the peak area and its uncertainty. Remember to save screenshots of your fitted peaks and their fitted area/sum (minimum of 8 peaks)

- Display rough peak energies by pressing "s"

- Click and drag on the x-axis to zoom in, zoom out by pressing "o"

- Click and drag on the y-axis to zoom in, zoom out by pressing "o" or right-click on the y-axis and click “Unzoom”

- Click on the left and click on the right side of the peak to set the fitting boundaries

- Fit by pressing "f"

- Save a screenshot of your fitted peak and its area in the terminal

- Remove all markers by pressing "n"

- Zoom in and repeat for 7 more peaks

- Quit GRSISort with ".q"

**Step 8.** In the RootEffi.C script, edit the peak areas and area uncertainties obtained from the peaks you fitted.

Remember that whenever you edit a script, you should save it and close ROOT/GRSISort to run it again.

**Step 9.** To run RootEffi, paste in the command line:

    grsisort -l RootEffi.C

**Step 10.** Save your edited script and your new efficiency curve

**Step 11.** In one file, submit screenshots of your fitted peaks (minimum of 8 peaks), your edited RootEffi script, and your efficiency curve :-)

***More analysis tools at*** https://github.com/GRIFFINCollaboration/GRSISort/wiki/Interactive-Analysis
