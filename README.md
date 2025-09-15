# ADK Agent Types

This repository contains examples of three different types of agents that can be built using the ADK (Agent Development Kit).

## Looping Agents

Looping agents are used for iterative processes where a task is repeatedly refined until a certain condition is met. The example in `loopingagents.txt` demonstrates a document writing and refinement process.

- **`InitialWriterAgent`**: Creates the first draft of a document.
- **`CriticAgent`**: Reviews the document and provides feedback for improvement.
- **`RefinerAgent`**: Updates the document based on the critic's feedback.

This loop continues until the `CriticAgent` is satisfied with the document and signals the loop to exit.

## Parallel Agents

Parallel agents allow for the concurrent execution of multiple agents. This is useful when different tasks can be performed independently and their results combined later. The `parallelagents.txt` file shows a stock analysis example.

- **`FundamentalAnalyst`**: Analyzes the fundamental aspects of a stock (e.g., financial health, valuation).
- **`TechnicalAnalyst`**: Analyzes the technical aspects of a stock (e.g., price trends, chart patterns).

These two agents run in parallel, and their combined analysis provides a more comprehensive view of the stock.

## Sequential Agents

Sequential agents execute a series of agents in a predefined order. The output of one agent becomes the input for the next, creating a pipeline. The `sequenceagents.txt` file illustrates a code generation workflow.

- **`CodeWriterAgent`**: Generates Python code based on a user's request.
- **`CodeReviewerAgent`**: Reviews the generated code for correctness, readability, and other quality aspects.
- **`CodeRefactorerAgent`**: Refactors the code based on the reviewer's comments.

This sequence ensures that the final code is of high quality and has been reviewed and improved.
