# Decomposition - Main Types

- Breaking problems into subproblems.
- Instead of step by step you are getting it to make subproblems

- Least-to-Most
- One Step Least-to-Most
- Multi Step Least-to-Most
- Plan-and-Solve
- Program of Thought


## Least to Most
 -  Decompose into smaller sub-problems
 - Solve these problems sequentially
 - Can be used with zero or few-shot

## One Step Least to Most
 - similar to zero shot CoT

### Example Prompt
To find the solution, first decompose the problem into separate sequential sub-problems. Then iterate to solve each and use it to answer the next.

## Multistep Least to Most

LLM returns a list of subquestion
THen give all those subquestions for final answer

## Plan and Solve

### Example Prompt
Let's first understand the problem and devise a plan to solve it. Then, let's carry out the pland and solve the problem step by step.

## Program of Thought
- good for programming tasks
- bad for semantic reasoning tasks
### Example Prompt
What sum results if you add up all the numbers from 1 to 100?

Please write easily understandable code that could be used to answer this question.
