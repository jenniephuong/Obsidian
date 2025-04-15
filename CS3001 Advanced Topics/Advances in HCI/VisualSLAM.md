what is VisualSLAM
- a type of SLAM system (early SLAM system (1986-now))
- uses ==vison sensor data== e.g. cameras (computer vision) to determine the position of the camera within the environment and map out the environment instead of relying on sensors like LIDAR
- uses feature detection to track key visual features across multiple frames
    - e.g. one type is MonoSLAM (single camera) developed in 2007, but can involve multiple cameras e.g. stereo camera, omnidirectional camera

how does visualSLAM work 
- ![[Pasted image 20250310170814.png]]

what is triangulation
- geometric process to estimate the 3D postion of a feature point in the world based on its projection from two or more camera views

what are the advantages of visualSLAM
- cost-effective - cameras can be more affordable that lasors
- wider field of view - cameras can see more so are better at detecting dynamic objects in AR or VR
- versatility - adaptable and can be used in drones, robots, anything for indoor navigation of AR and VR

how many features need to be extracted or observed for visualSLAM
- as many as possible, observing enough points can provide both structure and motion (camera path and scene structure)

what are some applications of visualSLAM
- e.g. Roombas, build a map of the surrounding to understand the scene, more features on the scene map give it a better understanding of the scene
- e.g. testing furniture in the environment by placing a sofa in the scene, need to first understand the scene![[Pasted image 20250310170859.png]]

what challenges are there for visualSLAM
- requires a camera moving through an unchanged scene and performs poorly for continually moving environments
- not suitable for person tracking, gesture tracking - high movement makes triangulation difficult
- outdoor tracking is not as good, illumination (lighting) inconsistencies
- cameras not always as precise as using lasers for LiDAR
- need to be done in a feature rich area (lots of edges and corners) and not in open or sparse areas otherwise less accurate mapping is created