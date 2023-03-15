# Strategies To Identify Similar Images/Measure The Similarity Of Images
### Pixel-wise Comparison/Pixel-by-pixel Comparison
- Sometimes, you may encounter situations in which a pixel-by-pixel comparison fails, but where a 
  visual inspection of the baseline and the image under test reveals no discernible difference. 
  This can occur, for example, when the display hardware used during testing differs from that 
  which was used during the baseline capture.
### Keypoint Detection Comparison/Image descriptors/feature detectors
- Many descriptors were developed for images, their main use is to register images/objects and search for them in other scenes.
- A keypoint detection comparison technique is an alternative. This technique is based on the 
  Scale Invariant Feature Transform (SIFT) algorithm, which transforms an image into a collection 
  of feature vectors, each of which is invariant to image scaling, rotation, translation, noise, 
  and other possible “corruptions” of an image. Therefore, a keypoint detection comparison 
  technique can be used to perform reliable matching between a baseline image and an image under 
  test in situations where you cannot be assured of a pixel-by-pixel identical match.
- Scale Invariant methods, SURF is a speed-up and open version of SIFT, SIFT is proprietary.
- **SIFT and SURF**: These are Scale Invariant methods, SURF is a speed-up and open version of 
                   SIFT, SIFT is proprietary.
- **BRIEF, BRISK and FAST**:These are binary descriptors and are really fast (mainly on processors                              with a pop_count instruction) and can be used in a similar way to SIFT and SURF. 
- **Histogram of Oriented Gradients (HoG)**:This is rotation invariant and is used for face detection...
### Sum Square Difference
- Template Matching is linear and is not invariant to rotation (actually not even robust to it) 
  but it is pretty simple and robust to noise such as the ones in photography taken with low 
  illumination.
  $$S_{sq} = \sum_{(n,m)\epsilon N} (I(n,m)-J(n,m))^2$$
- Normalized:
   $$\frac{S_{sq}}{\sqrt{\sum{I[n,m]^2\times[n,m]^2}}}$$
- OpenCV Template Matching.
### Cross-Correlation
              $$C_{crr} = \sum_{(n,m)\epsilon N} (I(n,m)\times J(n,m))^2$$
- Normalized:
              $$\frac{C_{crr}}{\sqrt{\sum{I[n,m]^2\times [n,m]^2}}}$$
### PHASH

### K-Mean Clustering

### Convolutional Neural Networks
- I know you don't want to used NN's but I think it is fair to point they are REALLY POWERFULL, training a CNN with Triplet Loss can be really nice for learning a representative feature space for clustering (and classification).
- Check Wesley's GitHub for a example of it's power in facial recognition using Triplet Loss to get features and then SVM to classify.
- Also, if your problem with Deep Learning is computational cost, you can easily find pre-trained layers with cats and dogs around.
- 
### Famous Measures:
- SSIM Structural similarity Index
- L2 Norm (Or Euclidean Distance)
- Mahalanobis Distance

### References
- https://datascience.stackexchange.com/questions/48642/how-to-measure-the-similarity-between-two-images
- 
