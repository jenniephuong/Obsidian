> a 3x3 rigid transformation of ==translation== and ==rotation== (based on the 6 Degrees of Freedom) aka. localisation and orientation The rotation element of the rigid transformation is nonlinear. The rotation element contains applying cosine and sine operations, which cause the nonlinearity

pose estimation needs to be done at each timestep 

what are the 6 degrees of freedom
- refers to the number of ways an object can **move** through a 3D space
- include 3 degrees for ==translational== movement and 3 degrees for ==rotational== movement
    - VR headsets can come in 3-DOG or 6-DOG
        - 3-DOG = a fixed position where the headset can track rotational movement of the headset but not translational
        - 6-DOG = tracks whether a user has both rotated or moved their head forward or back or up or down or side to side. a user can move around a virtual object

Inaccurate pose estimation in the mixed reality pipeline can lead to augmentation jumps.

what is an augmentation jump 
- a significant change in pose between frames that causes the virtual element's augmentation to jump - jarring, disorienting experience

Augmentation jumps can be happened due to a significant change in the optical sensor’s pose between frames causing a larger error. This error leads to augmenting the virtual object incorrectly in every frame, which looks like the object jumps, which can lead to cybersickness and discomfort.

#flash 