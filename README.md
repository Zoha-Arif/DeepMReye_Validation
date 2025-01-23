# Title
DeepMReye Validation

# Leaders
Ashley Hao (@HaoXin529), Elton Cross (@Ellieecross), Zoha Arif (@Zoha-Arif)

# Collaborators
Sophia Vinci-Booher (@svincibo)

# Project description
DeepMReye is a neuroimaging tool that uses deep learning to estimate gaze patterns directly from functional MRI (fMRI) data. Unlike traditional eye-tracking methods that measure eye-gaze using external hardware (i.e., eye-tracking cameras), DeepMReye measures eye-gaze using the signals from eyeball voxels captured in MRI scans. Our goal is to investigate whether DeepMReye measurements align with measurements recorded using in-bore eye-tracking data. If the DeepMReye and in-bore eye-tracking measurements align, DeepMReye could serve as an alternative method for participants who have only MRI data but lack eye-tracking information and the analysis of existing MRI datasets that lack eye-tracking measurements. Such investigations could offer insight into how the neural correlates of attention and visual processing are modulated by gaze behavior.

# Link to project repository/sources
https://github.com/Zoha-Arif/DeepMReye_Validation

# Concerete goals with specific tasks for Brainhack Vanderbilt 2025
Clone the repository (https://github.com/DeepMReye/DeepMReye) and run the test.
-Clone the repository.
-Navigate to the directory and install the required dependencies.
-Run the test scripts using the example data provided by DeepMReye to verify the set up is complete and all components function correctly.

# Investigate whether the gaze patterns derived from DeepMReye align with data from traditional eye-tracking tools.
-Use DeepMReye to extract eyeball voxel signals. (Note that the fMRI data have already been motion corrected.)
-Apply the pre-trained DeepMReye model to the extracted eyeball voxels to predict gaze positions.

# Compare DeepMReye results with available eye-tracking data to evaluate accuracy.
-Plot gaze trajectories for both methods on the same plot.
-Provide statistical summaries of alignment metrics (e.g., RMSE, correlation coefficients).
-Advanced move: Compare the DeepMReye and Eye-tracking timelines and highlight areas of agreement and discrepancies between the two eye-gaze measurements.

# Open-Source Documentation and Resources.
-Write guides for data preprocessing and DeepMReye setup.
-Include examples of comparative analysis with traditional eye-tracking data.
-Develop FAQs and troubleshooting guides

# Potential future work:
Development and Validation of DeepMReye: Implement a proof-of-concept model to estimate gaze patterns from fMRI data.
-Fine-tune the DeepMReye deep learning model
-Validate the model's accuracy across multiple datasets.
-Document performance metrics and areas for improvement.

# Good first issues
Issue one: Set up the repository and ensure the environment for running DeepMReye. https://github.com/DeepMReye. Test the installation process and report any issues or gaps in instructions. Explore the project's directory structure and understand the purpose of key files.

Issue two: Run existing scripts on small sample fMRI datasets to understand how the tool works and document the process for new contributors.

Issue three: Identify areas in the documentation that could be clarified or expanded. Add beginner-friendly explanations for complex concepts or workflows.

# Skills
Machine Learning (e.g., Deep Learning libraries like PyTorch)
Version Control (Git, Github)

# Onboarding documentation
https://github.com/DeepMReye
(This might be a good/alternative option: https://github.com/cpp-lln-lab/bidsMReye)

https://www.nature.com/articles/s41593-021-00947-w
https://github.com/DeepMReye/DeepMReye/blob/main/notebooks/deepmreye_example_usage.ipynb

# What will participants learn?
Participants will learn how to use neuroimaging tools like DeepMReye to infer gaze positions from MRI data. Additionally, they will develop skills in creating visualizations to interpret gaze data and neural activity using both DeepMReye and traditional eye-tracking data.

# Public data to use
Participants will use MRI and traditional eye-tracking data collected by the LAND Lab at Vanderbilt University.

DeepMReye sample data can be found here: https://osf.io/mrhk9/

fMRI and eye-tracking data for this project, specifically, can be found here: https://osf.io/suak8/

# Number of collaborators
4

# Credit to collaborators
Contributors will be credited in the GitHub repository and acknowledged in all future works related to the project. If the contribution shows significant promise, they may be invited to participate in a related research project with the hope of moving towards a publication.

# Image

Screenshot 2025-01-12 at 12 43 40 PM

# Project Summary
Use DeepMReye to estimate eye gaze patterns directly from functional MRI (fMRI) data.

# Type
coding_methods, method_development, visualization

# Development status
1_basic structure

# Topic
deep_learning, MR_methodologies, neural_decoding, reproducible_scientific_methods

# Tools
FSL, other

# Programming language
Matlab, Python

# Modalities
eye_tracking, MRI

# Git skills
1_commit_push, 2_branches_PRs
