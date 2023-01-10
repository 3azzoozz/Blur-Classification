Blurring is a form of reducing the bandwidth of an image.
It can be identified by many indicators:
- Fourier transform
- Edge detection filters (Laplacian, Sobel, Scharr, .. ).
- adding blur to the image itself and subtracting the result from the original image (For blurry images, the difference will be much smaller).

For this task, I used edge detectors and several blur filters to collect the necessary features of each image, as well as some transformations to determine the high and low frequencies in the image (Discrete wavelet transform, Butterworth filter (high and low)). After that, 3 classifiers were tested:
CatBoost, Random Forest and Neural Network Classifier. All have achieved excellent results.
CatBoost has the highest AUC and accuracy.
