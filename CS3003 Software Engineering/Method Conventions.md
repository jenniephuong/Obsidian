what method conventions should be used for clean code
- **minimise the number of parameters**
- **method callers and callees should be close together in the source code**
    - If one method calls another:
        - Keep those methods vertically close in the source file
        - Ideally, keep the caller right above the callee
        - We tend to read code from top-to-bottom, easier to read the code
- use the **same concepts** across the codebase `e.g. fetchValue() getValue()`, don’t mix these keywords or will cause confusion. just choose one.
- use **opposites** properly `e.g. add/remove, start/stop, begin/end, show/hide`


#L7_CleanCode 