# DeepLesion-Segmentation-with-TensorFlow-Python
A repository for the analysis of CT Scan slices and lesion annotations. Through this code, lesion mask labels can be created and adjusted, TF Record data can be produced, and Mask Region-based Architectures can be utilized (Inception-Resnet V2 was used).

This code is meant to be used with DeepLesion data and TensorFlow Object Detection API in Python.

Train_test_split can be used to split the available CSV data into two data sets

The 3D Mask Propagation file can be used to create mask annotations through statistical analysis of image pixels. Through specifying parameters, it can also be used to interpolate and produce intermediate slice annotations through a volume.

The generate_tf_records_new file is used to take the data produced by 3D Propagation and convert it into data readable by TensorFlow Object Detection API.

Inspection of these Records can be done through the inspect_records file.

After producing this data, it can be fed into TensorFlow ODAPI. We have supplied some basic files for the usage of ODAPI in the X folder.
