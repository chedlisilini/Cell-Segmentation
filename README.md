Nuclei of U2OS cells in a chemical screen
Accession number BBBC039 · Version 1

Example images
example image	example image
example image	example image
Description of the biological application
This image set is part of a high-throughput chemical screen on U2OS cells, with examples of 200 bioactive compounds. The effect of the treatments was originally imaged using the Cell Painting assay (fluorescence microscopy). This data set only includes the DNA channel of a single field of view per compound. These images present a variety of nuclear phenotypes, representative of high-throughput chemical perturbations. The main use of this data set is the study of segmentation algorithms that can separate individual nucleus instances in an accurate way, regardless of their shape and cell density. The collection has around 23,000 single nuclei manually annotated to establish a ground truth collection for segmentation evaluation.

Images
This data set has a total of 200 fields of view of nuclei captured with fluorescence microscopy using the Hoechst stain. These images are a sample of the larger BBBC022 chemical screen. The images are stored as TIFF files with 520x696 pixels at 16 bits.

Github repo

 images.zip (77.9 MB)

A small fraction of the images in this dataset overlap with the BBBC038 collection, which is the Data Science Bowl 2018 dataset. Not all images in this dataset were included in the DSB 2018 challenge to avoid a dominant number of fluorescent images for the competition. The BBBC038 collection has more variety of experimental conditions, whereas this dataset comes from a single high-throughput experiment with a large number of perturbations.

Ground truth  Foreground background button F Biological labels button B Outlines button O Counts button C
Ground truth annotations are stored as PNG files encoding masks of independent nuclei: if two nuclei touch, they are labeled with a different color. These annotations need to be decoded into labelled matrices to be used as ground truth. Example code for decoding masks can be found in this gist.

The images have been split in three subsets: training, validation and test. A metadata package contains files with the names of the images in each of these subsets. We suggest to use the same data partitions for any experiments, making the results comparable in future research. Example code to run and reproduce evaluation results can be found in the UNet4Nuclei repository. This repository has code for preparing the dataset as well as for training U-Nets and evaluating the results.

 masks.zip (2.8 MB)

 metadata.zip (18 KB)

For more information
Please contact the Imaging Platform.

Published results using this image set
This dataset has been used for evaluating the performance of Deep Learning models. More details of the evaluation framework in this bioRxiv preprint by Caicedo et al. 2018.

Recommended citation
"We used image set BBBC039v1 Caicedo et al. 2018, available from the Broad Bioimage Benchmark Collection [Ljosa et al., Nature Methods, 2012]."

Copyright
CC0Copyright: CC0. To the extent possible under law, the various contributors of the imagesets have waived all copyright and related or neighboring rights to BBBC039v1.
