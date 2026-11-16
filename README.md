# PFF-Internalization-by-Exclusion
---README---
Image J macro

Macro Name:
Macro for PFF exclusion for Internalized_v0.4

Image format
.tif

Image type:
Multichannel Z- projections. 


Macro Description. 

This macro is used to quantify internalized 488-PFF by removing surface-bound PFF signal identified by 2F11 staining.
This macro is used routinely to quantify antibody binding or positive signal on neurons, using a neuron mask such as MAP2 or fluorescent fill (ex. GFP, mCherry, TdTom). 

To use, all images with unique identifiers must be in the same folder. (If files other than TIF are in the same folder, it will cause the macro to stop. 

Users must indicate:

    Directory with Images to Analyze 
    Output Folder. Create a new folder before starting. This will contain the verification images and csv for results 
    Experiment info:
	  Experiment name
	  Pixel Scale. Current Scale 0.10049847 is the value for our Microscope Images (Andor Dragonfly) 
	  Number of Channels 
	  File index, tif 

Channel Assignment

	-Choose the Channel for A (Neuron mask), B (Internalized puncta to measure)C(Surface Puncta)
	-Method for Threshold. 
		Thresholding Methods
		 Manual
		 Set Value
		 Auto
		 From CSV. (If each image requires a different threshold value, a CSV with the names of the files and individual threshold values can be used) 

	-Name of Channels. Indicate the name of your markers. 
	-Puncta Overlap. Percentage of B that overlaps with C to be removed. 
	-Puncta Size for B and C.



-Analysis
	CSV file with quantification areas and Verification images for the thresholded masks, and the signal inside the ROI will be saved in the output folder
