# OCTA Vessel Segmentation Dataset

This repository is the official dataset for "COCTA: A Cortex Vessel Segmentation Benchmark using Optical Coherence Tomography Angiography"@*ISBI25*.

[Dataset](https://drive.google.com/file/d/1VlTNv5LO2H__y1DJiHelAjHV92zxBDER/view?usp=sharing)

#### Label indexes

- `1`: Vessel
-  `>1`: Ignored area (too noisy)

#### Naming format

{image|mask}\_{image_id}\_{`layer_id`}.tif

- `layer_id`:
  - `XXX_layer1.tif` is from `Layer1`.
  - `YYY_layer2.tif` is from `Layer2`.
  - `ZZZ_layer12.tif` is from `Layer12`.
- The same sample usually has three images: `image_321_layer1.tif`,  `image_321_layer2.tif`, and `image_321_layer12.tif`. `Layer12` is only available when both `Layer1` and `Layer2` are available.

Image RoI: Need to crop 10% of the left area used for scan-arm reset, as it has low SNR.

#### Compliance with ethical standards

All experimental procedures for animals related to the dataset used in this work were approved by the Institutional Animal Care and Use Committee of Stony Brook University. The data was collected under Stony Brook IACUC #252462_TR002.

#### Contact

jiaxren@cs.stonybrook.edu

hling@cs.stonybrook.edu

yingtian.pan@stonybrook.edu

#### Acknowledgment

This work was partially supported by NIH grants 1R21DA057699 (CD, YP, HL), 1RF1DA048808 (YP) and 2R01DA029718 (YP), and partially supported by NSF grants IIS-2331769 (HL).

The main annotation tool is [WEBKNOSSOS](https://home.webknossos.org).
