# Skin-Lesion-Classification
This GitHub repository contains image classification models for skin lesions using the ISIC dataset. The purpose of this project is to provide pre-trained models and code for classifying skin lesion images using four different models: ResNet152, VGG19, DenseNet201, and SqueezeNet1.1.

---
# Skin Lesion Image Classification

This GitHub repository contains image classification models for skin lesions using the ISIC dataset. The purpose of this project is to provide pre-trained models and code for classifying skin lesion images using four different models: ResNet152, VGG19, DenseNet201, and SqueezeNet1.1.

## Dataset
The models in this repository are trained on the ISIC dataset for the years 2019, 2018, and 2017. You can access the dataset for each year using the following links:
- [ISIC Dataset](https://challenge.isic-archive.com/data/)

## Accuracy on ISIC 2019 Train & Test Dataset 

| Model         | Mel Accuracy | BCC Accuracy |
| ------------- | ------------ | ------------ |
| ResNet152     | 95.78        | 96.46        |
| VGG19         | 95.33        | 95.82        |
| DenseNet201   | 95.11        | 97.43        |
| SqueezeNet    | 92.63        | 93.57        |


## Usage
To use the models for classification tasks, follow these instructions:

1. Clone the repository:
   ```
   git clone https://github.com/error9098x/Skin-Lesion-Classification.git
   ```


3. Download the pre-trained model files (.pkl) from the following locations:
   - [ResNet152 Model](https://www.kaggleusercontent.com/kf/129800036/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..wbmqcbfmypY_PEswXiDj6g.WRnILm3qGM56jOxD8xe2cO1-tRSIR_MQKcbFxscWYJV6n2JqaRsE72aFD1vecMbNIAkmQkpUFgN86fgn95kFh1MzVP4z5FWRCceKsUCOlE-gF5KcFkq2xcIhv_zf27HXXNv0JtLD06ypZuEWJf7fxfkMHY7_IciMyWO1xbZ06w1RgHp84h0mbMkzyTQ5f4u_ReclwrN7NKUoCbCyBgFkNybT_hNegujj0HuWFoh1TFhD-_s-kGb_c4GDt5apo0jgvlU-ENcm-try0ox00IdVps5ASRlcdCT9kcPKKsGxCAhAL4twAtAC5-XeMVeu8ERpBTh4A239AS4pg7HFT4Tea8JPABaBB1TPkYgQlEtHXKt7ayQ579E50j4Ag3bW5tiwi7aFx8Jyzgff6seA4gW_kWtP62eCMFCpOswMoXsIhg7ZuyvBlk4N6AzhFINDY6A9pEJs0ETa0cT-vFY9gRxwSE286FKnMzQ-aEX2ZqmBC0nKI8QuJb9688HiPEuBF14nMdFONbrG0bDSltfTOdLokZIYYbrBgDrJmrOpUUYpgmZNycawQ4K-pdOaxD0fH6kpjOl1rUH5YEel_2uSPsdRlo_4IujlANKNpPQA_LnmJ1v4CBEZvMsM2TqIy8iICZhMaFGvM17xErQLQQNa_5a4CnK7AnURGE5J05hKUQx_kK0.mG1h8xLX_1DQ_GJLxsrTBA/skinlesion_resnet152_only_two.pkl)
   - [VGG19 Model](https://www.kaggleusercontent.com/kf/129800489/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..xCNAK2NPoHOvDE4xooorew.U_YfQX7sF3gzdEGCtJJgPlfLDqjCV4F0gascYoB1jhcYPV-iLuIKnDAaXIVYSG_o_c76ukNtS_1JLumjLZDNZsAA4oXuu4osK2bapUs5V4TsVYNuZyXrWkHjG2ORXPUw0c_YwGDZDe8GC1xkvLz2D_cvgGNl65U27lu8J5reMfM79ijiQgnZa1C9p1y2KXEKG0OTwni9lvQ-uJAPyRRFdAtSScLXHYBQERCAP9oFub5FtC6vzaJAHKLoGpq2_59vnpdT-b89E0kkPY2ITT6GGxLOtSMgb7K-PG8TOvfhKFtB6NgoSl4ttPtYj9UX06GBRhMzTWhIyul-wXMn5oglZ8amSR0A64XwHdBewVCqT69Akqrbk9fl1Mrz2YqYrpuIU_byoDc0HPXy0z3553-6fE6bNlwTjTt1ECdEO5geQw4_QZhL0KD3o3oqpVSSP4FHNkf6RQxT3Zvq9LiJzHPeQaKOwoDSUUSN-JJ89CbpnPQLXv-NfWLHdhP5-xuw6qGG3GnL83bze2QI9yr2fCJ8lCgChjBFgngJug723VoxoMeAT9_QBzTAL6NHv2yyonPsKbTYFY6b7Pak9cHnYRPkGTRyBDgf3yBLpULxa9RlxhDan8C9dnyaY6m7ZelVX-zi2tyVMXS22XUj0-vq6zs_CA.TzRulYyqL-AVccr-cmF12Q/skinlesion_resnet152_only_two.pkl)
   - [DenseNet201 Model](https://www.kaggleusercontent.com/kf/129800321/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..fB48Pqd1h2UDEfs7ztiykQ.4gB63GIsrKodt60UbHEI_RchLQ9ciAKZofeH8juOJ5s-3EnVsEjT7layO9rPz1WdKb4NRlbXPlCXQnuucGS3Hq5XjZxeDP3xeISIBkF_xhXZHKFL1Z3NSFZuPnQfv2QgqIIAaub76WzRCq85uJXCFVEUWE0Vmy5s1oksqLCTQ4gqs6a7Sm1xpvZJW-07HRzwafHukCauqhFhPYff7pj57A9d0WyZg5Q4O9QVv-fJzrMoe6pzCpOmOPFU39VJYsO3qsGIp-xieNmbaSo7zgQT0_n-prvXBFkkVyb3js-9sgDfKm1g94JSKFp-RPY_y7HrJ6CXw-bwRfUnbwCbg2WmjCSz-wEpj73UIEfRVWCpgoq50_T2UupOQXJ3aN59uSfOmdnbvnp8n7gFQ8NjkPjYiWjrXW-Su4cFCH3t6CMLaYKYG-BpAfNyVm_-Q_jBXKlTHguNzy8sZCMxj4SGW0JGedMzazE35VRJnBstb50WRR337LpwljZIGZDipdnEjSuUpkqqW26N4v1F_oxAOmGOKg6ZtCpuLgEtPcwv-pxba-Opx3Ia5NED1K4cV31zpn_K1C251psFP8fE2jkZU4shQi52QqUhfvV7L8f1mmzXvLizEcmihI4lRnsFGBUnfcJlCpplk6lPWDujnHM_XVO4LMi5ZfaVXEUSbdLGvtZvjmg.M0roC4R--eoeSGe3bonDNg/skinlesion_densenet201_only_two.pkl)
   - [SqueezeNet1.1 Model](link-to-model-file)

4. Place the downloaded model files in the `models` directory.

5. Open the Jupyter Notebook (.ipynb) file for the desired model:
   - [ResNet152.ipynb](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/ISIC%202019%20Notebooks/isic2019-resnet152%20(1).ipynb)
   - [VGG19.ipynb](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/ISIC%202019%20Notebooks/isic2019-vgg19.ipynb)
   - [DenseNet201.ipynb](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/ISIC%202019%20Notebooks/isic2019-densenet201.ipynb)
   - [SqueezeNet1.1.ipynb](SqueezeNet1.1.ipynb)

6. Follow the instructions in the notebook to train or evaluate the model.

## Evaluation Metrics
The following evaluation metrics are provided for each of the four models:

- ROC Curves:
  - [ResNet152 ROC Curve](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/Images/ISIC2019Metrics/ResNet152/roc_curve_resnet152.png)
  - [VGG19 ROC Curve](Images/ISIC2019Metrics/Vgg19/roc_curve_VGG19.png)
  - [DenseNet201 ROC Curve](Images/ISIC2019Metrics/densenet201/roc_curve_DENSENET201.png)
  - [SqueezeNet1.1 ROC Curve](link-to-roc-curve-image)


- Precision-Recall Curves:
  - [ResNet152 Precision-Recall Curve](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/Images/ISIC2019Metrics/ResNet152/precision_recall_curve_resnet152.png)
  - [VGG19 Precision-Recall Curve](Images/ISIC2019Metrics/Vgg19/precision_recall_curve_VGG19.png)
  - [DenseNet201 Precision-Recall Curve](Images/ISIC2019Metrics/densenet201/precision_recall_curve_DENSENET201.png)
  - [SqueezeNet1.1 Precision-Recall Curve](link-to-precision-recall-curve-image)

- Accuracy Metrics:
  - [ResNet152 Accuracy Metrics](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/Images/ISIC2019Metrics/ResNet152/accuracy_resnet152.png)
  - [VGG19 Accuracy Metrics](Images/ISIC2019Metrics/Vgg19/accuracy_VGG19.png)
  - [DenseNet201 Accuracy Metrics](Images/ISIC2019Metrics/densenet201/accuracy_DENSENET201.png)
  - [SqueezeNet1.1 Accuracy Metrics](link-to-accuracy-metrics)

- Confusion Matrices:
  - [ResNet152 Confusion Matrix](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/Images/ISIC2019Metrics/ResNet152/confusion_matrix_resnet152.png)
  - [VGG19 Confusion Matrix](Images/ISIC2019Metrics/Vgg19/confusion_matrix_VGG19.png)
  - [DenseNet201 Confusion Matrix](Images/ISIC2019Metrics/densenet201/confusion_matrix_DENSENET201.png)
  - [SqueezeNet1.1 Confusion Matrix](link-to-confusion-matrix-image)

## Hugging Face Demo
You can try out the image classification models using the Hugging Face demo available at the following link:
- [Hugging Face Demo](https://huggingface.co/spaces/Hzjsjs/Skinlesion)
![Hugging Face Demo Screenshot](https://github.com/error9098x/Skin-Lesion-Classification/blob/main/Images/HuggingFace/hugginface.png)

---


