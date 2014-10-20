# Data Pipeline for Management and Publication of XROMM Experimental Data

Faculty Stakeholder: Callum Ross, PhD  

RCC Project Staff:
* Jason Voigt
* Simon Jacobs
* Richard Williams


# Objective

The RCC is working with Callum Ross to streamline the collection and publication of XROMM (X-ray Reconstruction of Moving Morphology) datasets.  XROMM is a new, morphology-focused approach to the study of joint biomechanics. It makes possible both the precise visualization and measurement of the interactions of articular surfaces within joints.

This project aims to create a semi-automated data pipeline from the Ross Lab, where X-ray motion trial data is captured and analyzed, to an XMA (X-ray Motion Analysis) Portal hosted by the RCC, where this experimental data can be made discoverable and accessible to the larger research community.

XROMM datasets are large and costly to acquire.  In addition to creating a streamlined research workflow for the Ross Lab, our XROMM dataset publishing pipeline enables the the re-use and re-purposing of these valuable research assets.


# Background

### XROMM

XROMM (X-Ray Reconstruction of Moving Morphology) is a new method for investigating skeletal kinematics, utilizing 3D imaging technology for visualizing and analyzing rapid skeletal movement in vivo. It combines three-dimensional models of bone morphology with motion data from biplanar x-ray video to create highly accurate re-animations of skeletal movement.

Bone motion data comes from two high-speed, biplanar x-ray movies. Bone morphology data comes from a 3D computer model of the bone surfaces (derived from CT, laser scanning, or MRI). This motion and shape data can then be used together to generate an XROMM animation. Rigid body kinematics inferred from the x-ray movies are applied to the skeletal models to re-animate the actual movement that was performed by the individual subject at the time of recording.

[XROMM hardware image]

[Caption: Diagram of mobile C-arm fluoroscopes, retrofitted for high-speed imaging. New 30-cm image intensifiers have been installed and the original cameras have been replaced with high-speed video cameras. A standard international (size 5) soccer ball is included for scale.]

[XROMM Ross Lab sample image]

[Caption: XROMM rhesus macaque mastication experiment.  Credit: Courtney Orsbon, PI: Callum Ross]

### XMA Portal

The XMA Portal is a web environment for the management of X-ray Motion Analysis (XMA) data developed at Brown University.  The XMA Portal serves as a powerful tool for organizing, searching, and disseminating XROMM experimental data.  As a component of the University of Chicago XROMM project, the RCC will be hosting a local instance of the XMA Portal.

[XMA Portal image]

[Caption: Data organization within the XMA portal. Repositories contain several studies and these studies may be associated with one or more PIs and the user who is conducting the experiments.]


# Data Pipeline

For each XROMM experiment, data is generated from multiple source machines
within the Ross Lab.  Data sources associated with each experiment can include x-ray video, neurophysiology data, electromyography data, force recordings, and anatomical models.  Metadata detailing the nature and provenance of each
experimental trial is also collected.  Any newly acquired experimental data is
transferred from the Lab to Midway on a nightly basis.  Raw data files are
securely stored on the Midway storage system and associated metadata is logged
in the XMA Portal's backend database, in order to expose new trial data via the
XMA Portal's web interface.


# Summary

The development of the XROMM data pipeline at the University of Chicago creates a streamlined research workflow that efficiently combines data storage and management on Midway with the ability to package and publish these research datasets using the XMA Portal.  This project facilitates reproducible analyses of XROMM datasets by leveraging the storage and computational capacity of the Midway computing environment.  This effort also promotes collaborative research by allowing rapid access to XROMM experimental data through the XMA Portal.
