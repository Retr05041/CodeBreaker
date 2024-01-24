# CodeBreaker
GA POC

## Info
Genetic Algorithm proof of concept

Language: C# (.Net Core 7.0)

Goal: Create a Genetic Algorithm to find a code of random numbers with a length of `X` faster on average than brute force.

## How the GA works
1. Generate a random 4 digit code.
2. Generate a beginning random population of size `X`
3. Evaluate fitness
4. Select best `Y` parents based off fitness
5. cross over parents & Mutation (till generation is full)
6. Return to step 3