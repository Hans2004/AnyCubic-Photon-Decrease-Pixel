# AnyCubic-Photon-Decrease-Pixel
A simple command line utility that can adjust the pictures in a .photon file to fit design dimensions more closely.

When printing with the Anycubic Photon printer at the optimum exposure time, some light from the edge pixels bleeds through. This causes objects to be 100um wider in the XY dimensions, and holes to be 100um smaller in the XY dimensions. Objects are perfectly sized in the Z dimensions.

This utility reads a photon file and trims off all the edge pixels from each layer. That way all horizontal dimensions come out perfectly.


The utility does not use any external libraries, thus it can be compiled as follows:

g++ main.cpp -o decreasePixel

Usage: decreasePixel infile.photon outfile.photon

The Linux executable can be downloaded as a single file from the Releases section.
There is also a zip file that contains the program (with some extra dll's) for Windows.
