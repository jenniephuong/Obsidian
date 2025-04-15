what is a ==registration error== 
- An error in the localisation and orientation estimation - causing a misalignment between the virtual elements and the real world environment (incorrect pose) during the tracking process causing some distortion
	impact: ruins immersion, 
	- e.g. 'swimming' objects, objects that are meant to be still start to move
	- e.g. misaligned objects, objects in the wrong place 

what causes registration errors
- system delay
- optical distortion - lenses (especially with a wide field of view) or displays used in HMD can create geometric distortions that affect how the virtual element is perceived e.g. pincushion vs barrel distortion
- ![[Pasted image 20250414151459.png]]
- tracker measurement error e.g. incorrect depth calculations or sensors not working due to poor illumination or rapid movement
- calibration errors - incorrect device calibration cause the virtual elements to be misplaced 


how can a registration error be fixed
- a registration error can be rectified by using an image distortion function, which is meant to correct the projection matrix.  
- make sure that one correctly calibrates all the optical sensors in the mixed reality headset.


trying to translate a 3D space into a 2D space that still looks like a 3D space 
![[Pasted image 20250310170007.png]]
- the marker has 3D coordinates in a physical space   
- the camera has its own coordinates in the 3D space
- based on these coordinates, the transformation of the marker is calculated to project the virtual object onto the 2D screen coordinates, but this can offset from the ideal screen coordinates (black vs. red dot) from what you actually see on the screen
- image distortion function is applied to fix this 