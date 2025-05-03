**L1_intensities File Processing**

This document describes the processing of the `L1_intensities.hdf5` file using Python and the `h5py` and `pandas` libraries. The primary goal was to extract relevant data from the file and convert it into a more accessible CSV format.

**Key Steps:**

1.  **File Inspection:** The `L1_intensities.hdf5` file was inspected to identify its structure and contents. This involved examining the groups and datasets within the file.
2.  **Dataset Extraction:**
    * The following datasets were extracted and converted to individual CSV files:
        * `straighten_worm_intensity_median`
        * `trajectories_data_valid`
    * The `INT_PROFILE` dataset, located within the `provenance_tracking` group, was also extracted to a CSV file. This dataset contains a single scalar value.
3.  **Output Format:** All extracted data was saved as CSV files, with column headers derived from the dataset structure (where applicable).

**Libraries Used:**

* `h5py`:  For reading and navigating the HDF5 file structure.
* `pandas`:  For creating and exporting dataframes to CSV files.

**Purpose:**

The processing steps outlined here were performed to make the data contained within the `L1_intensities.hdf5` file more readily available for analysis.  The conversion to CSV format allows for easier manipulation and exploration of the data using standard data analysis tools.
# L1_intensities
Data extraction of the L1_intensities results file
