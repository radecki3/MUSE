**DISCLAIMER**

This work was done with the oversight of Dr. Tony Wong at UIUC, who was my research advisor and directed much of my work shown here. Dr. Wong made many contributions to the code, some of which are unseen in this repo. 

This repository contains some code for processing ESO MUSE data. All MUSE data that was used is courtsey of NSF, ESO, and Dr. Anna McLeod at Durham University. Dr. Peter Zeidler at STScI created the MUSEpack Python package and assisted with our correction efforts.

We also made use of NSF NOIRLab's DEMCELS data and GAIA DR3 data, which are both publicly accessible.

**OUTLINE**

There are a couple of notebooks which highlight some of the main points of progress for our work. They are not necessarily final or complete representations of our work but are examples of some steps we took. 

*MUSEWCS*: There are fairly significant WCS offsets in all of the MUSE data cubes. This is very noticeable when compared to GAIA or HST data. This notebook highlights some of the major steps we took in correcting those. 

*MUSEFLUX*: There also exist significant flux offsets in the MUSE data, with noticeable "banding" and different characteristic background flux values for each tile. This notebook compares MUSE to DEMCELS, which includes the same region, and has much more normalized flux across N44. We decided to rescale the MUSE tiles to roughly match the DEMCELS flux. 
