# Brain-Tumor-Radiogenomic-Classification

This repository code, and information related to the Brain Tumor Radiogenomic Classification project. The project aims to predict the genetic subtype of glioblastoma using MRI (magnetic resonance imaging) scans to detect the presence of MGMT promoter methylation, a significant genetic biomarker crucial for brain cancer treatment.

Project Overview

Brain cancer, specifically glioblastoma, poses a significant threat to patients' lives. This project focuses on leveraging machine learning techniques on MRI scans to predict the MGMT promoter methylation status, aiding in less invasive diagnosis and customized treatment strategies for brain cancer patients.

Dataset

The dataset used in this project consists of three cohorts: Training, Validation (Public), and Testing (Private). Each case is represented by a dedicated folder identified by a five-digit number. Within each case folder are four sub-folders containing structural multi-parametric MRI (mpMRI) scans in DICOM format:

Fluid Attenuated Inversion Recovery (FLAIR)

T1-weighted pre-contrast (T1w)

T1-weighted post-contrast (T1Gd)

T2-weighted (T2)

Folder Structure

train/: Contains training files, each top-level folder representing a subject. Note: Exclude cases [00109, 00123, 00709] during training due to unexpected issues.

train_labels.csv: File containing the target MGMT_value for each subject in the training data.

test/: Contains test files structured similarly to train/. Predict the MGMT_value for each subject in the test data.

The data originates from the RSNA-ASNR-MICCAI BraTS 2021 Benchmark on Brain Tumor Segmentation and Radiogenomic Classification. For citation purposes, reference the dataset as follows:

Citation:

U.Baid, et al., “The RSNA-ASNR-MICCAI BraTS 2021 Benchmark on Brain Tumor Segmentation and Radiogenomic Classification”, arXiv:2107.02314, 2021.
