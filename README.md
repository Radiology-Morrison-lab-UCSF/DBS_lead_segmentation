# DBS_lead_segmentation
Tool to segment Deep Brain Stimulation leads without artifacts on CT scans and register to MNI152 1mm space. Then based on user defined atlas space, overlapping regions in atlas space and segmentations are defined. 

The input CT scan MUST be in .nii.gz file format. The output is a binary mask of the segmented electrode.

# Instructions
1. Clone this repository to your local space.
2. Create an output directory for your files. 
3. Create a virtual environment and pip install the following dependencies: numpy, matplotlib, opencv-python, itk-elastix, fsl-py, SimpleITK-SimpleElastix, tensorflow, nibabel. 
4. Open a new terminal and activate the virtual environment.
5. Change your current working directory to the folder "code".
6. To use the tool, run the following command $ bash run.sh input_file_path output_file_path (Be sure to replace input_file_path and output_file_path with the paths to your files). Threshold = electrode pixel value. 

**Note atlas.py code may need to be edited based on which atlas template user requires (see code) 
