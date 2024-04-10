```c#
CurrentSolution <-- initalState
finalSolution <-- Backtrack(currentSolution)

Function Backtrack(currentSolution)
    If currentSolution is complete then
        return currentSolution
var <-- SelectUnassignedVariable(currentSolution)
For each value in OrderDomainValues(currentSolution, var) do
    If value is consistent with currentSolution then
        Add{var = value} to currentSolution
        Inferences <-- INFERENCE(var, currentSolution)
        If inferences ≠ failure then
            Add inferences to currentSolution
            result <-- Backtrack(currentSolution)
            If result ≠ failure then
                return result
        Remove{var = value} and inferences from currentSolution
Return failure
```

