# DP

DP = Backtracking (Formatting smartly) + Caching (saving the required info in the process)

## General Steps

1. Identify the form/pattern
2. Identify the states (90% of the times this is the question asked)
3. Transition modeling.
4. Save/catch and Return
5. Code

## Recursion

``` C++
ll fib(n):
{
    // Base Case;
    if(n==0 or n==1)
        return 1;
    else
        return (fib(n-1) + fib(n-2));
}
```

**Always consider that we will get correct ans from what we have called using recursion**
**the only job we need to do is use that correct answer exactly and get our required ans from it;**
In this way we will get the perfect ans everytime without any worry.

Also always see recursion as a 1 to 1 interaction between our current state and 1 step smaller state;

Level, Choice, Check, Move;

1. Level: The way to iterate over all solution space(items) efficiently, or exploring all the possible options.
2. Choice: For the current level what possible moves/choices you have? or what what can you do from the current level.
3. Check: Out of all the choices for current level Which choices are valid and which are not? or which need to explored furhter.
4. Move: If a valid choices are there then move to each one of them to get to a new level and repeat all these steps...again.
