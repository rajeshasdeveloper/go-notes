-   Go doesn't have constructors as it does hide cost.
-   Factory functions are the functions that creates the value, initializes it for use, and returns it back to the caller. This is great for readability, it doesn't hide cost, we can read it, and lends to simplicity in terms of construction.
-   All the memory associated with the active frame **up** is valid.
-   When **main** making another call, it is going to wipe out all the data below the active frame.
-   By identifying the return type of the function, Go allocates the memory ans set the value in heap not in the stack, And now Garbage Collector needs to manage it as now the allocation is on heap (The stack has self-cleaning capability). Because of this there is a cost of performance.
-   Don't construct the variable as pointer semantics as it hides the readability and cost.
