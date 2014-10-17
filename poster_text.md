#Objective
The aim of this project is to create a data pipeline from the raw data streams generated in each XROMM laboratory experiment to the packaging and publishing of the data on the XMA portal.  Data sources associated with each experiment can include: x-ray video, neurophysiology data, electromyography data, force recordings, and anatomical models. This pipeline will permit these large and expensive-to-acquire data collections to be reused and repurposed by the community of researchers in a highly efficient manner.

#Background
###XROMM
XROMM is a 3D imaging technology for visualizing and analyzing rapid skeletal movement in vivo. It combines three-dimensional models of bone morphology with motion data from biplanar x-ray video to create highly accurate re-animations of skeletal movement.

Bone motion data comes from two high-speed, biplanar x-ray movies. Bone morphology data comes from a 3D computer model of the bone surfaces (derived from CT, laser scanning, or MRI). This motion and shape data can then be used together to generate an XROMM animation. Rigid body kinematics inferred from the x-ray movies are applied to the skeletal models to re-animate the actual movement that was performed by the individual subject at the time of recording.

[XROMM image and caption]

###XMA Portal
The XMA Portal is a web environment for the management of X-ray Motion Analysis (XMA) data developed at Brown University.  The XMA Portal serves as a powerful tool for organizing, searching, and disseminating XROMM experimental data.  As a component of the University of Chicago XROMM project, the RCC will be hosting a local instance of the XMA Portal.

[XMA Portal image and caption from Jason’s email]

#Data Pipeline
[Pipeline figure]
[Caption: High-level sketch of the semi-automated XROMM dataset production pipeline]

In this pipeline, data collected from multiple source machines during XROMM experiments will be transferred from the XROMM facility to Midway. This transfer of experimental will be run as an sbatch script that executes a set of rysnc commands nightly on Midway.  In addition to the raw data, metadata detailing each experimental trial and its associated datafiles will be archived in an SQL database on Midway.  The stored experimental data will be made searchable and accessible to the scientific community through the XMA Portal web interface hosted on Midway.
