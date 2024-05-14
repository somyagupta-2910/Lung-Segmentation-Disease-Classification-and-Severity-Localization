# lung-disease-segmentation-classification-localisation

### INTRODUCTION
Accurate and rapid diagnosis of respiratory diseases such as COVID-19 and viral pneumonia using chest X-rays (CXRs) is crucial for timely treatment and containment efforts. However, traditional diagnostic approaches often struggle with high variability in image quality and the subtlety of disease manifestations, leading to a significant rate of diagnostic errors. To address these challenges, this report presents a novel hybrid multi-stage network that initially segments the lung region in the CXR images, followed by classification and subsequent localization of the disease using Grad-CAM. This approach allows for focused analysis on relevant lung areas, enhancing the model's accuracy and reliability in diagnosing respiratory conditions.

### DATASET

For our project, we are using the [COVID-19 Radiography Database](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database). This comprehensive database contains chest X-ray images for three distinct classes: COVID-19, normal, and viral pneumonia. Specifically, the dataset comprises 3616 images of COVID-19 positive cases, 10,192 images categorized as normal, and 1345 images identified as viral pneumonia. This extensive collection allows us to train our diagnostic models effectively, ensuring robust performance in identifying and classifying these conditions.

### LITERATURE REVIEW
Recent advancements in deep learning, such as the U-Net model proposed by Ronneberger et al. (2015) [1] for precise biomedical segmentation and CNNs like VGG and ResNet for disease classification, have significantly enhanced lung disease diagnosis from X-ray images. The study by Teixeira et al. (2021) [2] highlights the effectiveness of these techniques, achieving notable diagnostic accuracy. Additionally, the use of Explainable AI methods such as Grad-CAM, introduced by Selvaraju et al. (2017) [3], enhances diagnostic transparency by visually explaining model decisions, improving reliability in medical imaging diagnostics.

### METHODOLOGY
Our approach involves a systematic progression through three stages: segmentation, classification, and localization. This structured workflow allows us to precisely isolate and analyze lung regions, identify pathological conditions, and visually highlight critical areas influencing diagnostic outcomes, thereby facilitating a comprehensive examination of CXR images.

### REFERENCES
1] W. Weng and X. Zhu, “U-Net: Convolutional Networks for Biomedical Image Segmentation,” IEEE Access, vol. 9, pp. 16591–16603, May 2015, doi: 10.1109/ACCESS.2021.3053408.

[2] L. O. Teixeira et al., “Impact of Lung Segmentation on the Diagnosis and Explanation of COVID-19 in Chest X-ray Images,” Sensors 2021, Vol. 21, Page 7116, vol. 21, no. 21, p. 7116, Oct. 2021, doi: 10.3390/S21217116.

[3] R. R. Selvaraju, M. Cogswell, A. Das, R. Vedantam, D. Parikh, and D. Batra, “Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization,” Int J Comput Vis, vol. 128, no. 2, pp. 336–359, Oct. 2016, doi: 10.1007/s11263-019-01228-7.
