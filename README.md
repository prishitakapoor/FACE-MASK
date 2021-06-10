# FACE-MASK
Face Mask is computer vision-based script to mask faces in images. It uses a dlib based face landmarks detector to identify the face tilt and six key features of the face necessary for applying mask. Based on the face tilt, corresponding mask template is selected from the library of mask. The template mask is then transformed based on the six key features to fit perfectly on the face. The complete block diagram can be seen below. MaskTheFace provides a number of masks to select from. It is difficult to collect mask dataset under various conditions. MaskTheFace can be used to convert any existing face dataset to masked-face dataset. MaskTheFace identifies all the faces within an image, and applies the user selected masks to them taking into account various limitations such as face angle, mask fit, lighting conditions etc. A single image, or entire directory of images can be used as input to code.
![image](https://user-images.githubusercontent.com/51163007/121483875-4b6f9200-c9ec-11eb-9587-ec4539522ac1.png)


# Features


# Support for multiple mask types
MaskTheFace supports various mask-types such as surgical, N95, cloth etc. Moreover, user can easily configure MaskTheFace for any new/custom mask type by following simple guidelines. More mask types are constantly being added to the tool.
![image](https://user-images.githubusercontent.com/51163007/121484023-778b1300-c9ec-11eb-94f5-091e368fcd89.png)


# Support for various mask variations
Various existing patterns and/or color overlays can be applied to existing mask types to create more variations of the masks. Moreover, users can easily add custom patterns following the guidelines provided
![image](https://user-images.githubusercontent.com/51163007/121484160-938eb480-c9ec-11eb-8003-bb882a273529.png)


# Support for both single and multi-face images:
MaskTheFace applies user-selected masks to all the faces present in the image.
![image](https://user-images.githubusercontent.com/51163007/121484210-a0130d00-c9ec-11eb-8b46-314775f5bb99.png)


# Wide face angle coverage
A wide range of fave tilt and angle is considered to apply proper mask to the faces. Based on the face angle, one of three templates is selected and applied.
![image](https://user-images.githubusercontent.com/51163007/121485101-81f9dc80-c9ed-11eb-816d-a58c0599b04d.png)


# Bulk masking on datasets
Any face dataset can be converted to masked faced dataset with a simple script. This is particularly useful when dealing wuth bulk images.
![image](https://user-images.githubusercontent.com/51163007/121485158-8de59e80-c9ed-11eb-856b-02bafc00c5ef.png)


# MFR2 Dataset
A small dataset of real-world masked faces of 53 identities and 269 images aligned and preprocessed. This dataset can be used to evaluate how well the simulated mask domain is transferred to real masks
![image](https://user-images.githubusercontent.com/51163007/121485278-ab1a6d00-c9ed-11eb-87ec-542ab1e7d6c7.png)


# Mask Types
Currently MaskTheFace supports the following 4 mask types
![image](https://user-images.githubusercontent.com/51163007/121486037-69d68d00-c9ee-11eb-9277-732aa347a7b2.png)


# Pattern variations
MaskTheFace provides 24 existing patterns that can be applied to mask types above to create more variations of the masks. Moreover, users can easily add custom patterns following the guidelines provided
![image](https://user-images.githubusercontent.com/51163007/121486082-72c75e80-c9ee-11eb-8efc-a012603ff1b5.png)


# Color variations
MaskTheFace provided script can be used to modify existing mask types in terms of color types to generate variations of existing masks.
![image](https://user-images.githubusercontent.com/51163007/121486127-7c50c680-c9ee-11eb-9ecd-2867804b3309.png)


# Color intensity variations
MaskTheFace provided script can be used to modify existing mask types in terms of color intensity to generate variations of existing masks.
![image](https://user-images.githubusercontent.com/51163007/121486168-85da2e80-c9ee-11eb-9fd8-29d014444879.png)


MFR2 Dataset
Masked faces in real world for face recognition (MFR2) is a small dataset with 53 identities of celebrities and politicians with a total of 269 images that are collected from the internet. Each identity has on average of 5 images. The dataset contains both masked and unmasked faces of the identities. The dataset is processed in terms of face alignment and image dimensions. Each image has a dimension of (160x160x3). Sample images from the MFR2 data-set and the mask distribution can be seen below. In the future we plan on expanding this dataset to contain more indetities and images.
![image](https://user-images.githubusercontent.com/51163007/121488104-6217e800-c9f0-11eb-8ddf-1ac824dbe283.png)

![image](https://user-images.githubusercontent.com/51163007/121488131-69d78c80-c9f0-11eb-9916-8e7f4c238424.png)

# Datasets
https://drive.google.com/file/d/1ukk0n_srRqcsotK2MjlFPj7L0sXcR2fH/view

# MFR2 Content
Folders with images of identities.

mfr2_labels.txt : Label text file with identity name, image number, and type of mask ground truth.

pairs.txt : Text file containing 848 positive and negative pairs to be used for testing
