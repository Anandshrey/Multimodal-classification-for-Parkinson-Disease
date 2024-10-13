# Multimodal Classification for Parkinson's Disease
Implements a multimodal model for categorizing participants as 'Normal' or 'Parkinson'. It utilizes multimodal data - tabular data and brain MRI images to make the classification.

## Overview
This study suggests a multi-modal diagnostic paradigm incorporating various data sources, including MRI scan images and tabular data having UPDRS (Unified Parkinson's Disease Rating Scale) scores from a 4-part UPDRS evaluation which assesses motor and non-motor aspects of daily living that get impacted due to Parkins's disease. The disease is often characterized by the degeneration of dopamine-producing cells in a specific region of the brain known as the substantia nigra. The image data to investigate this degeneration consists of mid-brain slices from T1 and T2 weighted MRI scans.  Utilizing multi-modal data fusion, our method employs the Vision Transformer model (ViT) for image analysis and a Gradient Descent model for tabular data. The study used the Parkinson's Progression Markers Initiative (PPMI) dataset, which included midbrain T1 and T2-weighted MRI images and UPDRS scores.

## Dataset
The data for this study was acquired from the PPMI database. The tabular data consists of UPDRS score totals from the four-part UPDRS assessment for 831 participants. The image data consisted of mid-brain MRI slices for the same participants. 

## Approach
A Late Fusion approach was used to combine the two modalities and build a multi-modal classifier
![LateFusion](https://github.com/user-attachments/assets/400e43e8-b1d0-49ca-be6b-8c5a92edcb65)

## Sections
### Reading Tabular Data
### Build and Test a Gradient Descent model to classify Tabular data
### Read Image Data
### Build and Test a Vision Transformer (ViT) model to classify Image data
### Define a function to average the predictions from the two models
### Make multimodal predictions using the function
### Evaluate the performance of the two unimodal models and the multimodal model
