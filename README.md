# Anomaly Segmentation in Retinal Images with Poisson-Blending Data Augmentation
# Abstract
Diabetic retinopathy (DR) is one of the most important complications of diabetes. Accurate segmentation of DR lesions helps early diagnosis of DR. However, due to the scarcity of pixel-level annotations and the large diversity between different types of DR lesions, the existing deep learning methods are very challenging in performing segmentation on retinal images. In this study, we propose a novel data augmentation method based on Poisson-blending (PB) algorithm to generate synthetic images, which can be easily adapted to other medical anomaly segmentation tasks to alleviate the training data scarcity issue. We also proposed a CNN architecture for the simultaneous segmentation of multiscale anomaly signs. The performances are compared with the state-of-the-art methods on Indian Diabetic Retinopathy Image Dataset (IDRiD) and e-ophtha datasets, both widely used in the research community. The results indicate that the proposed method significantly outperforms the state-of-the-art methods.
# 1. Prepare data. 
- The DR datasets we collected from [IDRiD dataset](https://doi.org/10.3390/data3030025) and [e-ophtha dataset](https://doi.org/10.1016/j.media.2014.05.004). You can download the datasets from [Baidu Netdisk](https://pan.baidu.com/s/1GTxq9EgBrAV-tUyOnLG8kA?pwd=6kft)(access code: 6kft) and decompress it to ["./original_data"](original_data). 
- The vessel segmentation dataset we used to trained a U-Net for getting vessel masks is in ["./vessel_seg"](vessel_seg). The weight file of trained model can be gotten from [Baidu Netdisk](https://pan.baidu.com/s/1LWtQo3Z-BMdLjhMVd5PSRA?pwd=ikrm)(access code: ikrm), and please put it into ["./vessel_seg/results"](vessel_seg/results). If you want to train a new model, please go to ["./vessel_seg/README.md"](vessel_seg/README.md) for details.
## 2. Environment
- Please prepare an environment with python=3.7, and then use the command "pip install -r requirements.txt" for the dependencies.

## References
* [Indian Diabetic Retinopathy Image Dataset (IDRiD): A Database for Diabetic Retinopathy Screening Research](https://doi.org/10.3390/data3030025)
* [Exudate detection in color retinal images for mass screening of diabetic retinopathy](https://doi.org/10.1016/j.media.2014.05.004)
