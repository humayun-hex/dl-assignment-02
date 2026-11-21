# Deep Learning Assignment 02

CNN architectures and controlled ablations on CIFAR-10.

## Reproduce the experiments

1. Open `cnn_assignment.ipynb` in Google Colab and choose a T4 GPU under **Runtime > Change runtime type**.
2. Run the notebook from top to bottom. The first cells write the Python modules and check the model structures.
3. The training cells use the same 12,000 training and 3,000 validation images for each model. The split seed is 42. The main runs use batch size 32, mixed precision and up to five epochs per fit. The optional seed 123 scratch runs are enabled.
4. The notebook selects a checkpoint by validation accuracy, then macro F1, then run ID. It records that choice before evaluating the original 10,000 test images once.
5. The final cell shows the curves and test results. The `experiment` directory contains the CSV, split indices and per run records.

The submitted `results.csv` records the measured Colab runs. The analysis is in the separate `CNN_Assignment_02_Report.pdf` submitted through the course portal.
