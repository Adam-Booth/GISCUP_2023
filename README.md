# SIGSPATIAL 2023

Team: Adam Booth, Richard Burke

Contact: a.booth2@newcastle.ac.uk, r.burke1@newcastle.ac.uk

Our solution is primarily based on the excellent research produced by Dumitru et al. in their paper 'Using DUCK-Net for polyp image segmentation' https://github.com/RazvanDu/DUCK-Net.

### Directory Structure

    .
    ├── src     # Contains three Python Jupyter Notebooks
    ├── data    # Expected to contain 2023 SIGSPATIAL Cup data files under '2023_SIGSPATIAL_Cup_data_files'
    ├── model   # Contains trained Tensorflow/Keras model for lake delineation model
    ├── lake_polygons_test.gpkg     # Lake polygons generated from the model and test data (submission)
    └── README.md

### How to Run

This repository contains three notebooks, 01_training_set_generation.ipynb, 02_model_training.ipynb and 03_test_lake_deliniation.ipynb. To reproduce the results achieved, run each of the three notebooks in numerical order.

This submission contains the final model we trained and can be used directly by only running 03_test_lake_deliniation.ipynb. To generate the model from scratch, you must run 01_training_set_generation.ipynb and 02_model_training.ipynb first.

Note: The notebooks automatically create directory structures within the data directory which stores intermediate data between the running of the notebooks. After running all three notebooks, the total size of the directory is **70GB** and therefore should be executed on a drive with adequate storage space.
