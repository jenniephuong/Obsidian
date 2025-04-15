not all comments are good or necessary. comments sometimes used to hide bad code
can be a sign of [[Tech Debt]] as people have left comments instead of refactored

what do comments show (according to Fowler)
- complicated code
- code that is in need of explanation but that actually needs restructuring rather than commenting

how should comments be done (according to Fowler)
- self-evident coding practices by making methods short, comments meaningful
- commenting the decision making process for the solution implemented i.e., why something is there, not what is does

#L3_SoftwareRefactoring 

what are the trade-offs to comments for [[Clean Code]]
- helpful or damaging, if they must be included, minimize them
- poor or inaccurate comments are worse than no comments - need [[Refactoring]]
- comments can lie from being outdated
- the code should speak for itself, comments only added when code can’t be self documenting (Daniel Read)![[Pasted image 20241120101250.png]]

#L7_CleanCode

what are five guidelines to comments
- don’t comment poor code, rewrite the code
- do warn of consequences in the code `e.g. “this code will take a while to run”`
- do emphasize important points in the code `e.g. “sometimes the data input has leading space”`
- don’t include “noise” in you comments `e.g. “// this is declaration of an int called “day” int day;`
- don’t copy and paste comments, because you’ll always forget to make the necessary changes [[Cut, copy-paste]]

#L3_SoftwareRefactoring 