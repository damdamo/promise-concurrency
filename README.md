# Promise example for Hero nets

Original code can be found on:
https://javascript.info/promise-chaining

The code uses the GitHub API to collect users' information and print avatars.
In our case, we choose two GitHub profiles and we want to print the avatar in a specific order.

Each file can be opened separately in a browser to see the result.
- *concurrencyProblem.html*: Introduce the original problem, where two avatars are printed in a non-determinism way.
- *badSolutionConcurrencyProblem.html*: Show a solution to this concurrencyProblem in introducing a global variable. A problem appears if the second profile is the first to be printed. In this situation the second profile is not printed.
- *solutionConcurrencyProblem.html*: A solution where avatars are always printed as we wish. We use the `promiseAll` function to resolve this issue.
