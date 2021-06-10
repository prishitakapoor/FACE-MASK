# FACE-MASK
Face Mask is computer vision-based script to mask faces in images. It uses a dlib based face landmarks detector to identify the face tilt and six key features of the face necessary for applying mask. Based on the face tilt, corresponding mask template is selected from the library of mask. The template mask is then transformed based on the six key features to fit perfectly on the face. The complete block diagram can be seen below. MaskTheFace provides a number of masks to select from. It is difficult to collect mask dataset under various conditions. MaskTheFace can be used to convert any existing face dataset to masked-face dataset. MaskTheFace identifies all the faces within an image, and applies the user selected masks to them taking into account various limitations such as face angle, mask fit, lighting conditions etc. A single image, or entire directory of images can be used as input to code.


Features

Support for multiple mask types
MaskTheFace supports various mask-types such as surgical, N95, cloth etc. Moreover, user can easily configure MaskTheFace for any new/custom mask type by following simple guidelines. More mask types are constantly being added to the tool.

Support for various mask variations
Various existing patterns and/or color overlays can be applied to existing mask types to create more variations of the masks. Moreover, users can easily add custom patterns following the guidelines provided



Support for both single and multi-face images:
MaskTheFace applies user-selected masks to all the faces present in the image.

Wide face angle coverage
A wide range of fave tilt and angle is considered to apply proper mask to the faces. Based on the face angle, one of three templates is selected and applied.



Bulk masking on datasets
Any face dataset can be converted to masked faced dataset with a simple script. This is particularly useful when dealing wuth bulk images.

MFR2 Dataset
A small dataset of real-world masked faces of 53 identities and 269 images aligned and preprocessed. This dataset can be used to evaluate how well the simulated mask domain is transferred to real masks

