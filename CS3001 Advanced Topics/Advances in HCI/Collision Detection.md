> the detection of a collision (contact) between the interaction model / real world objects / or other virtual elements, and the virtual element to prevent objects moving through each other, ensuring they react realistically 

sometimes using direct interaction where 10 collidable fingertips are used can cause unexpected and unpredictable collisions

3D object manipulation can be done using a bounding box to provide better depth through proximity shader
- shaders - visual indication that collision detection is about to be initiated
- ![[Pasted image 20250310183714.png]]

(hands, visual tracking, collision detection)

computationally demanding
- collisions are calculated when the collider on the fingertip interacts with the bounding box 

what is a bounding box 
- a cube that encapsulates a virtual object to indicate that it can be interacted it
- handles often added to the orders and edges of the bounding box so that the object can be scaled and rotated 
- makes it more intuitive to interact with ![[Pasted image 20250310184153.png]]

#flash 