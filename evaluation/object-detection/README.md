# Object Detection – Evaluation Results

This directory contains all evaluation outputs for the object detection module described in the thesis.  
The results are based on the final YOLOv12s configuration and dataset composition outlined in the methodology section.

## Dataset Reference
The underlying dataset, including the full documentation of its creation, preprocessing scripts, and the final train/validation/test splits, is available in the  
[**`object-detection`** directory of the repository](https://github.com/ToHauser/FootballAI/tree/main/object-detection).
This folder was linked in the methodology chapter during the explanation of the underlying data basis.


## Directory Structure

- **`yolo12s_train_val_results/`**  
  Contains the training and validation curves of the best-performing YOLOv12s model, including precision, recall, mAP curves, and confusion matrices.

- **`yolo12s_test_results_tile/`**  
  Contains the evaluation results on the dedicated test set using the tile inference approach. This folder includes per-class metrics and output visualizations.

- **`train_test_val.ipynb`**  
  A complete Jupyter Notebook detailing the training, validation, and testing workflow, including all hyperparameters, dataset paths, and evaluation scripts.

## Notes
The test set evaluation is the only component of the system validated against ground truth labels.  
All other evaluation modules in the repository are based on the six-minute amateur match video provided in the main [evaluation directory](https://github.com/ToHauser/FootballAI/tree/main/evaluation).
