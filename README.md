# Advanced AI Model Test Suite

This repository includes a public markdown prompt set for evaluating AI models across a broad range of capabilities.

## File

- [ai-model-test-prompts.md](C:/JV/Prompts/ai-model-test-prompts.md)

## What It Tests

The prompt set contains 25 prompts designed to evaluate:

- coding
- math
- logic
- reasoning
- instruction following
- creative writing
- generalization
- synthesis
- ambiguity handling

The prompts are designed to reward more than fluent wording. A strong model should show accuracy, depth, clarity, adaptability, and honest handling of uncertainty.

## What Makes This Useful

- It covers both technical and non-technical tasks.
- It includes exact-format and constraint-heavy prompts, which are good for catching brittle models.
- It mixes direct problem solving with open-ended judgment tasks.
- It tests whether a model can shift tone, audience, and abstraction level.

## Recommended Usage

- Run one prompt at a time in a fresh chat when possible.
- Keep system instructions consistent across models if you are comparing them.
- Save the full output, not just pass or fail notes.
- Score both the final answer and how well the model followed the prompt.

## Suggested Evaluation Criteria

- `Accuracy`: Are the claims correct?
- `Instruction Following`: Were all constraints obeyed?
- `Clarity`: Is the response easy to understand?
- `Depth`: Does it go beyond shallow surface content?
- `Adaptability`: Can it adjust style and explanation level well?
- `Robustness`: Does it handle ambiguity and tradeoffs honestly?
- `Usefulness`: Would the response help a serious user?

## Suggested Scoring Method

One simple approach is to score each prompt from 1 to 5 on each criterion:

- `1`: poor
- `2`: weak
- `3`: acceptable
- `4`: strong
- `5`: excellent

You can also add short notes for:

- hallucinations
- missed constraints
- shallow reasoning
- unjustified certainty
- formatting failures

## Good Comparison Practices

- Test multiple models on the same prompt wording.
- Avoid giving hints unless hints are part of the benchmark.
- Compare not only best-case answers, but also consistency across several prompts.
- Pay special attention to instruction-following tasks, because many models sound strong while failing exact requirements.

## Intended Audience

This prompt set is useful for:

- model evaluators
- prompt engineers
- AI product teams
- developers comparing models
- anyone building an informal benchmark

## Notes

- The prompts are written in markdown so they are easy to copy, reuse, and expand.
- The set is broad rather than domain-specific, making it useful for general-purpose model evaluation.
- You can extend it later with scoring sheets, answer keys, or model-specific notes if needed.

