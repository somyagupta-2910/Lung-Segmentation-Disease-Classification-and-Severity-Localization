# lung-disease-segmentation-classification-localisation

### PROBLEM STATEMENT
Accurate detection of lung diseases from X-ray images is hindered by the inclusion of non-lung tissues and artifacts. This project proposes a targeted three-step approach: precise lung field segmentation using models like U-Net and PSP-Net with various backbones, disease classification through focused algorithms such as ResNet, CoatNet and Vision Transformers, and critical decision-making visualization with Grad-CAM. This method aims to improve diagnostic accuracy and interpretability, enabling earlier and more precise identification of lung pathologies.

### LITERATURE REVIEW
Recent advancements in deep learning, such as the U-Net model proposed by Ronneberger et al. (2015) [1] for precise biomedical segmentation and CNNs like VGG and ResNet for disease classification, have significantly enhanced lung disease diagnosis from X-ray images. The study by Teixeira et al. (2021) [2] highlights the effectiveness of these techniques, achieving notable diagnostic accuracy. Additionally, the use of Explainable AI methods such as Grad-CAM, introduced by Selvaraju et al. (2017) [3], enhances diagnostic transparency by visually explaining model decisions, improving reliability in medical imaging diagnostics.

### DATASETS & MODELS
Datasets: COVID-19 Radiography Database, Montgomery County X-ray Set, Classification Dataset Models: UNet, PSP-Net, DeepLab V3+, ResNet, CoatNet, Vision Transformer (with different backbones).

### METHODOLOGY
We will use segmentation models like U-Net and PSP-Net for lung segmentation from x-ray images, selecting the best-performing model to segment the lungs onto a numpy array. This segmented output will then be classified by models like ResNet or ViT to identify lung diseases, focusing only on lung features. Additionally, techniques such as Grad-CAM will be applied to visualize and assess the model's decision-making regions within the lung, aiding in the accurate identification and severity assessment of infectious areas.

### DELIVERABLES & EXPECTATIONS:
- A robust model pipeline capable of segmenting, classifying, and visualizing lung diseases from X-ray images.
- Achieve higher accuracy and precision in lung disease identification compared to current full-image analysis methods.
- Provide clinicians with visual aids using GradCAM to understand the AI’s diagnostic pathways, potentially increasing trust and usability in clinical settings.

### REFERENCES
1] W. Weng and X. Zhu, “U-Net: Convolutional Networks for Biomedical Image Segmentation,” IEEE Access, vol. 9, pp. 16591–16603, May 2015, doi: 10.1109/ACCESS.2021.3053408.
[2] L. O. Teixeira et al., “Impact of Lung Segmentation on the Diagnosis and Explanation of COVID-19 in Chest X-ray Images,” Sensors 2021, Vol. 21, Page 7116, vol. 21, no. 21, p. 7116, Oct. 2021, doi: 10.3390/S21217116.
[3] R. R. Selvaraju, M. Cogswell, A. Das, R. Vedantam, D. Parikh, and D. Batra, “Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization,” Int J Comput Vis, vol. 128, no. 2, pp. 336–359, Oct. 2016, doi: 10.1007/s11263-019-01228-7.
