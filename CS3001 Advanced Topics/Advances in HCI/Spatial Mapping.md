> the process of a mixed reality device mapping the real space, for the device to create an understanding of the scene aka. understand the position and orientation of different objects or users in the environment - responsible for placing and moving the virtual elements of the scene.


how does spatial mapping work
- creates a mesh (triangle based geometric structure) over the real environment like a fishing net to map out the shapes and layouts of the surroundings
- ![[Pasted image 20250310172944.png]]
- mesh is created using computational geometry and computer vision like [[VisualSLAM]]
- done because system doesn’t understand real world measures like cm or meters

what does spatial mapping allow us to do
- **visualise virtual objects** - place and position them onto the surroundings using [[Pose Estimation]]
- **allow virtual objects to navigate** - let them move around the surroundings (the object may be an agent or a character like a moving chibi, not just a static object)
- **perform physics simulations** - e.g. a bouncing object, an object jumping or matching gravity. 
- **become occluded (hidden)** by items in the real world e.g. hiding behind a table

what are the limitations of spatial mapping
- work well indoor, but not outdoors