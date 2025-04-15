https://dl.acm.org/doi/10.1145/3544548.3581292

Physical manikins and VR are already being used independently for skills training - what about a hybrid MR approach? 
- specifically for first responders to train them in a more hands on way that is both functionally effective and cost effective

Using real tools and hands to interact with virtual elements over-layed onto a manikins
- more akin to augmented virtualisation? as the manikins and the trainee are placed in a virtual accident scene

AR is not realistic enough

Normal VR approaches are top down - mainly observation of virtual interactions, lacking haptic feedback
- eliminates risk, liability, and injury 
- already VR approaches for practicing surgery, first aid treatment, learning anatomical knowledge, medical ethics training 
- focus on learning through theory and immersion rather than through application
- unable to track small tools in the VR process 

Hybrid approach places focus on realism

how is this tech setup
- greenscreens and chroma keying - laying multiple video streams to create a composite scene based on colour, the mannequin is chroma-keyed so virtual elements can be over-layed even though the manikins is real 
- LiDAR sensors to capture depth information 
- printable fiducial markers attached to real objects like stethoscope so that the HMD can track them, and object collision scripts used to calculate interactions between the objects and the mannequin to trigger other effects like sound when using stethoscope
- HMD has pass through cameras and a scent emitter, video feed can be screen shared 

how was it evaluated 
- quantitative results on technology acceptance and presence, and user surveys with likert scale
- qualitative data from workshops and post MR experience discussions
- GSR for galvanic skin response to measure arousal  

pros 
- medical realism
- haptic feedback 
- high immersion - more intuitive using hands than using controllers 
- trainees had high acceptance of the technology
- trainees had high amount of physical presence and self-presence, ability to produce stress in the participants which is realistic to the scenario 
- lower cost and more repeatability than hiring actors to play mass casualty  simulations 

cons 
- tracking and audio issues 
- researchers creating MR experiences have blind spots e.g. providing only a subset of first responder tools for them to use, not having a full mannequin with clothing:  which unintentionally limits the realism of the scenario compared to what the people interacting with the MR experience might expect  
- graphical glitches with transparent elements 
- people might not understand how to interact with the virtual elements at first - solve by adding a tutorial