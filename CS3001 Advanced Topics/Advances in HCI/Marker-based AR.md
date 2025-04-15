#### introduction to markers 

what is a marker 
- a reference point to superimpose digital content onto the physical environment. 
- made up of distinct patterns that the camera can recognise using computer vision, usually independent of the physical environment e.g. paper-based marker.

what are the two types of marker 
- black and white marker
- colour based, image marker

https://medium.com/@deepanshut041/introduction-to-fast-features-from-accelerated-segment-test-4ed33dde6d65
https://arxiv.org/pdf/2106.01055


how does the algorithm detect the marker
- binarization - converting any image (colour or not) into a binary image where each pixel is either 0 or 1
- greyscale - converting images so that each pixel has an intensity value between 0 and 255
- edge detection - identifies and edge (change in intensity between two regions) within an image to define the marker’s shape, e.g. using Canny edge detection algorithm
- corner detection - pinpoint where edges meet (change in intensity in multiple directions), e.g. using Harris Corner Detection or FAST (Features from Accelerated Segment Test)
- surface colour discontinuity - identifying abrupt changes in colour, since black and white markers have high contrast
- illumination discontinuity - changes in lighting or shadows or glare

what is the pipeline for rendering objects with marker-based AR 
![[Pasted image 20250310165814.png]]
- the object is superimposed onto origin of the marker, and rendering is a continuous process over every timestep - changing the position of the marker changes the position of the object

what is the function for calculating a marker's transformation 
- 3D transformation = position and rotation relative to the camera

what is a common error that can occur with marker tracking
- [[Registration Error]]

what are the pros of marker-based AR
- easy to use and implement
- efficient and real time performance (low latency)
- feature-based tracking, which is very stable

what are the cons of marker-based AR
- can sometimes loose the augmentation due to lighting, occlusion, fast movements that the processor cannot detect in time
	- e.g. what if this was being used for a camera for a surgery has the limitation of movement
- if the camera moves away from the marker, the virtual content disappears
- does not work with reflected light
- marker must have strong borders and contrast - no smooth colour transitions
- does not work with occlusion

what is the pipeline for using image-based markers to render virtual elements 
- continuous tracking and tracking stability - involves more sophisticated feature detection and pose calculation (aka. transformation) algorithms![[Pasted image 20250310170313.png]]

why is image based AR challenging
- needs to keep continuous track of feature points in each frame with respect to next frame - noise making the AR less accurate
- may be too many features to extract - before it was just simplified edges and corners but with images there are so many edges and corners to extract per timestep
- needs to keep continuous track of image pose over time, thus detects outliers (pose calculation/pose estimation) - computationally expensive calculations
- frame rate could be slow, the optical sensor’s pose may change significantly between frames and cause augmentation “jumps” as it is augmented incorrectly in every frame and the virtual element’s position also jumps, can be disorienting for the user
- framerate drops significantly, this latency is not acceptable for humans, not efficient


#flash