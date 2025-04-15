> the number of immediate sub-classes a class has (breadth of a class hierarchy)

Inheritance based complexity metric 
- not as good as [[Depth in the Inheritance Tree of a Class (DIT)]] since NOC doesn’t promote method reuse, but closely related to DIT

![[Pasted image 20241104105313.png]]

what does a high NOC indicate
- high reuse of base class through inheritance
- base class needs more testing
- improper abstraction of parent class
- misuse of sub-classing, should instead combine subclasses and create another level of inheritance
- less faults as a result of high reuse

high NOC and [[Weighted Methods per Class (WMC)]] = complexity at the top of class hierarchy and it's impacting many descendant classes and could show poor system design, redesign required maybe

#L2_SoftwareMetrics 