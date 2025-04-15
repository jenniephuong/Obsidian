> estimates the camera parameters in the mixed reality head-mounted display device

mixed reality requires some device for usage 
- use ==see-through displays== (e.g. visual pro, occulus) like headsets
- headsets contain many image sensors, depth cameras, IR illuminators, colour video cameras, greyscale cameras → producing a video stream of what the user is wearing
- they have minimum specifications e.g. aspect ratio, resolution, and display rate that must be met to work properly

what are the base specs. for a mixed reality headset
- aspect ratio 3:2
	- Having four covers a wide coverage as the user needs to make sure they are able to see the surrounding environment as they can to avoid collision and as a driving simulator, being aware of the surrounding.
- resolution 2k
	- fluence the level of immersion of the driver and their ability to acquire awareness of the situation during the experience, pixelated breaks immersion
- display rate 120-240Hz
	- a refresh rate of less than 120 Hz would lead the driver to have motion sickness and discomfort, show high latency 
	- risk of augmentation jumps 
- having a depth and grayscale camera 
	- Depth camera allows device to measure the depth information and distance for the object from a 3D point and allows visual SLAM tracking. 
	- Grayscale camera which allows to capture grey images of the environment.
		- greyscale are more cost effective than colour cameras

what is sensor calibration 
- the device calibration process estimates the ==camera parameters== (aka. the camera’s orientation and translation) in an MR headset to establish an accurate relationship between a 3D point in the real world and the corresponding 2D projection image captured by the camera
- optical sensor calibration for MR headsets or AR devices is needed to avoid registration errors, correct distortion, produce precise measurements, but can be difficult to do

how does sensor / device calibration work
- using the required intrinsic properties to estimate and initialise the extrinsic parameters of the real world![[Pasted image 20250310172447.png]]

what are the intrinsic properties
- optical centre - the origin of the camera’s coordinate system
- scaling

what are the extrinsic properties
- refers to the location of the camera in the 3D scene
    - orientation aka. camera rotation
    - translation
- these properties are not always known

without proper device calibration, [[Registration Error]]s can occur 
