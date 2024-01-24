# CodeBreaker
GA POC

## Info
Genetic Algorithm proof of concept

Language: C# (.Net Core 7.0)

Goal: Create a Genetic Algorithm to find a code of random numbers with a length of `X` faster on average than brute force.

## How the GA works
1. Generate a random 4 digit code.
2. Generate a beginning random population of size `X`
3. Evaluate fitness based of possibel parents digits being in the same index as the code, e.x. Code: 1234, Possible Parent: 5674 ~ The fitness of the possibe parent is: 1, because the 4's are in the same position, else it counts as 0
4. Select best `Y` parents based off fitness
5. cross over parents incorrect code digits randomly with other parents incorrect code digits, and create random combinations of random numbers and correct digits to fill the rest of the generation to the size of `X`
6. Return to step 3