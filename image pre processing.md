
# Image-pre-processing

  Image pre-processing are the steps you take to convert the images in it's raw form into a form that your model is ready to use for tranning and inference. Images can be of different sizes, orientation, contrast level, image pre-processing is the data cleaning for the computer vision.
  
  As a Machine Learning Engineer, data pre-processing or data cleansing is a crucial step and most of the ML engineers spend a good amount of time in data pre-processing before building the model. Some examples for data pre-processing includes outlier detection, missing value treatments and remove the unwanted or noisy data.

Similarly, Image pre-processing is the term for operations on images at the lowest level of abstraction. These operations do not increase image information content but they decrease it if entropy is an information measure. The aim of pre-processing is an improvement of the image data that suppresses undesired distortions or enhances some image features relevant for further processing and analysis task. 

## Steps involved in image pre-processing
There are 4 different types of Image Pre-Processing techniques and they are listed below.

1. Pixel brightness transformations/ Brightness corrections
2. Geometric Transformations
3. Image Filtering and Segmentation 
4. Fourier transform and Image restauration


### 1. Pixel brightness transformations(PBT) 
  Brightness transformations modify pixel brightness and the transformation depends on the properties of a pixel itself. In PBT, output pixel’s value depends only on the corresponding input pixel value. Examples of such operators include brightness and contrast adjustments as well as colour correction and transformations.

  Contrast enhancement is an important area in image processing for both human and computer vision. It is widely used for medical image processing and as a pre-processing step in speech recognition, texture synthesis, and many other image/video processing applications

  #### There are two types of Brightness transformations and they are below.
  1. Brightness corrections
  2. Gray scale transformation

  #### The most common Pixel brightness transforms operations are
  1. Gamma correction or Power Law Transform
  2. Sigmoid stretching 
  3. Histogram equalization

  #### Two commonly used point processes are multiplication and addition with a constant.
  > g(x)=αf(x)+β

  The parameters α>0 and β are called the gain and bias parameters and sometimes these parameters are said to control contrast and brightness respectively.
  > cv.convertScaleAbs(image, alpha=alpha, beta=beta) 

  for different values of alpha and beta, the image brightness and contrast varies. 

### 2. Gamma Correction
Gamma correction is a non-linear adjustment to individual pixel values. While in image normalization we carried out linear operations on individual pixels, such as scalar multiplication and addition/subtraction, gamma correction carries out a non-linear operation on the source image pixels, and can cause saturation of the image being altered.
