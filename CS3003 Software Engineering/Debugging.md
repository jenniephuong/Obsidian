what are the debugging principles
- fix 1 thing at a time → not multiple problem fixes or changes at once, test hypothesis, change back if it doesn’t fix a problem
- question your assumptions → don’t assume simple small lines of code or mature products work e.g. libraries can have bugs e.g. [[Defensive Programming]]
- check recent code changes → bugs can be caused by latest code pushes
- use a debugger → breakpoints, memory watches, stack
- break complex calculations into steps → decompose conditional refactoring, the equation could be wrong or cast badly
- check boundary conditions → off by 1 for loops, ≤, ≥
- take a break → too close to the problem to see it
- explain the bug to others → helps retract steps and provide alternative hypothesis
- debug with a partner → new techniques, same pros as code reviews and pair, [[Mob Programming]]
- use outside helps → stack overflow

what are 2 types of debugging approaches
- [[Rubber Duck]] debugging
- [[Wolf Fence]] debugging


#L5_FaultProneness 