# ADAPT Example Data

Animated GIFs looking at 4D tomographs through the middle of the ITV, and an appendix to the 2025 communications engineering article as a word file.

Note that each "case" contains conventional (1320 projections over 240 seconds), STO600 (adaptive acquisition conventional reconstruction, 600 projections over 60 breaths) and STO200 (adaptive acquisition adaptive reconstruction, 200 projections over 20 breaths) images. Each case needs to be extracted from .zip seperately.

The ITV contour is shown in yellow, spine canal contour in blue (these contours are gnerally used by clinicians for patient alignment).

Note that the contours are directly from the planning CT and the patients have not neccesarily been aligned.

Each case is supposed to be representative of the study cohort, plus the worst STO200 image as quantified by CNR.

The file "simplestats.m" includes the underlying data and plotting code for some summary statistics/plots.

The "ADAPTcodes.zip" folder contains the matlab scripts used to perform the image reconstruction in the ADAPT study. Note these algorithms are implemented as calls to the elastix toolkit and Reconstruction Tool Kit (RTK) to do all the heavy lifting:

https://elastix.dev/

https://www.openrtk.org/

