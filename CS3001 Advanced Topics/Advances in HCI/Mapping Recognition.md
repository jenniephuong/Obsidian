> registers and recognises non-static elements of the real world, which allows one to communicate between the real world and virtual objects, and for collision detection and interactions 

the hand and fingertips are examples of a non-static element of the real world 

how can the headset do the mapping recognition 
- by tracking our hand - user’s hands are recognised and interpreted as left and right hand ==skeletal models==
- colliders and bounding boxes initialised
- collision detention algorithm is applied between the hands and the object to detect when the hand is about to interact with the virtual object

what is a collider 
- an object (e.g. box collider, sphere collider) which is visually rendered at the tip of each fingertip to provide better cues for near targeting, the sphere’s diameter should match the thickness of the index finger to increase touch accuracy

why are sphere colliders efficient 
- sphere matches the shape of the finger, higher **accuracy**
- rotationally invariant: changing the **rotation** doesn’t impact the collider and will not impact the effectiveness of the collision detection
- more **efficient** to calculate than rectangles or other things

how is mapping recognition applied to a hand 
- five ==colliders== are attached to the five fingertips of each hand skeletal model
- bounding box encapsulates the object to detect when hands enter the bounding box
- space between the collider and bounding box is measured
    - as soon as the collider approaches the object, collision detection is initiated
    - ![[Pasted image 20250310181507.png]]
- the hand is not virtual but there spheres on them are, the sphere can also be visualised

Detecting collisions and interactions between the user's hand and the virtual objects occurs at this stage 
- [[Collision Detection]]

Currently within HoloLens the collider on the user's fingertip is used to Help with interacting with the virtual element.