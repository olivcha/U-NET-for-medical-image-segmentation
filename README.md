# U-NET-for-medical-image-segmentation
U-Net neural network architecture developed based on Ronneberger, Fischer and Bronx's work ([2015](https://doi.org/10.48550/arXiv.1505.04597)) as a part of Computer Vision coursework at Imperial College London, taught by [@baiwenjia](https://github.com/baiwenjia). 

**Requirements**  
In order to run this code, you will need Jupyter-lab (https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html) and other libraries used. To install those, run the command as follows:

_`pip3 install [package_name]`_

**GPU resource**  
Due to pre-processing performed on images, this code will run on CPU.

However, to save training time, you may want to use GPU. In that case, you can run this notebook on Google Colab. On Google Colab, go to the menu, Runtime - Change runtime type, and select **GPU** as the hardware acceleartor.

**Dataset**  
This code uses dataset developed for the [Medical Segmentation Decathlon](https://doi.org/10.1038/s41467-022-30695-9). The original dataset can be found [here](https://goo.gl/QzVZcm). This dataset is provided under the [Creative Commons](https://drive.google.com/file/d/18dLVTJtkp052danMjzlirAgIsklT_Aem/view?usp=drive_link) license. The [dataset](https://www.dropbox.com/s/zmytk2yu284af6t/Task01_BrainTumour_2D.tar.gz) provided by Dr Wenjia Bai includes images for the first task of the MSD after pre-processing, including extraction of 2D image slices from T1-Gd contrast enhanced 3D brain volumes and downsampling of the images. The dataset consists of a training set and a test set. Each image is of dimension 120 x 120, with a corresponding label map of the same dimension. 

[1] Olaf Ronneberger et al. [U-Net: Convolutional networks for biomedical image segmentation](https://link.springer.com/chapter/10.1007/978-3-319-24574-4_28). MICCAI, 2015.  
[2] Zongwei Zhou et al. UNet++: A Nested U-Net Architecture for Medical Image Segmentation. DLMIA, 2018.  
