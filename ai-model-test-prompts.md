# Advanced AI Model Test Suite: 25 Strong Prompts

This prompt set is designed to evaluate an AI model across multiple dimensions, including coding, math, logic, reasoning, instruction following, creative writing, and generalization. The prompts are meant to reward accuracy, depth, clarity, adaptability, and honest handling of uncertainty.

## How To Use

- Run one prompt at a time for cleaner evaluation.
- Judge both answer quality and how well constraints are followed.
- Look for shallow confidence, missed edge cases, vague reasoning, and formatting failures.

---

## 1. Coding: Debugging With Edge Cases

You are given this Python function:

```python
def compress(text):
    result = ""
    count = 1
    for i in range(len(text)):
        if i < len(text) - 1 and text[i] == text[i + 1]:
            count += 1
        else:
            result += text[i] + str(count)
            count = 0
    return result
```

Tasks:

- identify the bug
- explain why it fails
- provide a corrected version with minimal changes
- give 5 edge-case tests
- state what the function should return for an empty string

Do not replace the approach unless necessary.

## 2. Coding: API Design With Tradeoffs

Design a REST API for a collaborative notes platform with:

- user accounts
- organizations or workspaces
- sharing permissions
- document version history
- comments
- search

Your answer must include:

- core endpoints
- example request and response bodies
- status codes
- authentication approach
- 3 design tradeoffs

## 3. Coding: Refactoring Judgment

Refactor this JavaScript function for readability and maintainability without changing behavior. Then explain what you improved and what you intentionally did not change.

```javascript
function x(a,b,c){if(a){if(b){return c.map(function(i){return i.id}).filter(function(j){return j!=null})}}return[]}
```

## 4. Coding: Algorithm Design

You are given a list of 10 million integers where every number appears exactly twice except for two numbers that appear once.

Design an efficient method to find the two unique numbers.

Your answer must include:

- the algorithm
- why it works
- time complexity
- space complexity
- one less efficient alternative and why it is worse

## 5. Coding: Test Planning

Write a compact but high-value test plan for a password reset feature in a production web application.

Include:

- happy paths
- authentication and authorization concerns
- abuse and rate-limiting cases
- token expiry and replay cases
- logging or observability checks

## 6. Math: Proof and Teaching

Prove that the sum of the first `n` odd numbers is `n^2`.

Then:

- explain the proof in simple language for a 12-year-old
- give a small numeric example
- name one common mistake a student might make here

## 7. Math: Applied Modeling

A tank contains 120 liters of saltwater with 18 kg of dissolved salt. Fresh water flows in at 4 L/min, and well-mixed solution flows out at 4 L/min.

Tasks:

- derive a formula for the amount of salt after `t` minutes
- calculate the amount after 30 minutes
- explain why the amount decreases the way it does

## 8. Math: Fermi Estimation

Estimate how many piano tuners there are in Chicago.

Show:

- your assumptions
- your reasoning process
- a low estimate
- a medium estimate
- a high estimate

Then say which assumption matters most.

## 9. Math: Error Analysis

A student claims:

> Since `sqrt(a + b) = sqrt(a) + sqrt(b)`, we have `sqrt(9 + 16) = 3 + 4 = 7`.

Explain:

- the exact mistake
- why the pattern feels tempting
- a correct way to check whether an algebra rule is valid
- one more example of a similar false rule

## 10. Logic: Knights and Knaves

On an island, knights always tell the truth and knaves always lie.

Person A says: "At least one of us is a knave."
Person B says: "A is a knight."

Determine who is a knight and who is a knave, and justify the answer step by step.

## 11. Logic: Deduction Under Uncertainty

Three friends, Ava, Ben, and Chloe, each own a different pet: a cat, a dog, and a parrot.

Clues:

- Ava does not own the cat.
- Ben does not own the dog.
- The person with the parrot is not Chloe.

Tasks:

- determine all assignments consistent with the clues
- say whether the answer is unique
- explain how you know

## 12. Reasoning: Correlation vs Causation

Ice cream sales and drowning incidents both rise during the summer.

Explain why this does not mean ice cream sales cause drowning.

Then give 2 real-world cases where confusing correlation and causation could lead to bad business or policy decisions.

## 13. Reasoning: Decision Framework

A startup has 6 months of runway left. Leadership is deciding whether to:

- build a new feature requested by current customers
- spend the time improving reliability
- cut costs and slow product development

Do not give a one-line recommendation. Instead:

- identify the key unknowns
- explain the tradeoffs
- propose a decision framework
- describe what evidence would most change your recommendation

## 14. Reasoning: Argument Evaluation

Evaluate this argument:

> "Remote work reduces office costs. Therefore, every company should be fully remote."

Your answer must identify:

- hidden assumptions
- overgeneralizations
- missing variables
- a stronger version of the argument
- the strongest objection to that stronger version

## 15. Instruction Following: Precision Constraint

Follow these instructions exactly:

1. Write exactly 4 bullet points.
2. Each bullet point must contain exactly 9 words.
3. The topic is staying productive while learning difficult material.
4. Do not use the words "focus", "study", "learn", or "distraction".

## 16. Instruction Following: Strict JSON

Respond in valid JSON only using this schema:

```json
{
  "title": "string",
  "summary": "string",
  "risks": ["string"],
  "score": 0
}
```

Task: Summarize the risks of launching a mobile app without analytics, crash reporting, or user feedback channels. Use a score from 1 to 10.

## 17. Instruction Following: Ordered Transformation

Take the sentence below and apply the transformations in order:

Sentence: "The quick brown fox jumps over the lazy dog."

Instructions:

1. Convert to uppercase.
2. Reverse the order of the words.
3. Remove the word "THE" wherever it appears.
4. Replace `DOG.` with `HOUND`
5. Output the final result as a single line only.

## 18. Creative Writing: Controlled Atmosphere

Write a scene of about 250 words in which a scientist opens a letter from their future self.

Requirements:

- emotionally restrained tone
- intelligent and quietly unsettling mood
- no cliches
- no explicit explanation of time travel
- end on an image, not an explanation

## 19. Creative Writing: Voice Differentiation

Write the same event twice: a city losing power during a thunderstorm.

- Version 1: literary fiction
- Version 2: hard-boiled noir

Each version should be 120 to 160 words and should feel clearly distinct in rhythm, imagery, and attitude.

## 20. Creative Writing: Constraint Storytelling

Write a short story under 300 words about first contact with non-human life.

Constraints:

- no dialogue
- no proper nouns
- no combat
- do not use the words "alien", "spaceship", or "planet"

The result should still feel vivid, consequential, and emotionally real.

## 21. Generalization: Rule Extraction

Given these examples:

- `glim -> glimmed`
- `trask -> trasked`
- `plone -> ploned`

Tasks:

- infer the transformation rule
- apply it to `mave`, `drint`, and `sproke`
- explain whether this is true generalization or pattern imitation

## 22. Generalization: Teaching Pattern Transfer

A teacher says:

> "Good explanations move from concrete example to general principle to practical use."

Use that teaching pattern to explain recursion to a beginner.

Your answer should visibly follow the pattern.

## 23. Generalization: Audience Adaptation

Create 3 analogies for how database indexes work:

- one for a child
- one for a business executive
- one for a software engineer

Keep the core idea accurate while adapting the framing to each audience.

## 24. Synthesis: Cross-Domain Analysis

A school wants to use AI to help teachers write quizzes faster.

Analyze the idea from these angles:

- technical feasibility
- educational quality
- ethics and bias
- operational rollout

Then give a balanced recommendation with concrete safeguards.

## 25. Robustness: Ambiguous Question Handling

Answer this carefully:

> "What is the best programming language?"

Requirements:

- do not give a universal answer
- identify at least 5 contexts where the answer changes
- recommend a language for each context
- explain the criteria for each choice
- note where reasonable experts may disagree

---

## Suggested Evaluation Rubric

- `Accuracy`: Is the answer factually, mathematically, or logically sound?
- `Instruction Following`: Were all required constraints obeyed?
- `Clarity`: Is the answer easy to follow?
- `Depth`: Does it go beyond obvious surface-level content?
- `Adaptability`: Can it shift across audience, style, and abstraction level?
- `Robustness`: Does it handle ambiguity, tradeoffs, and edge cases honestly?
- `Usefulness`: Would the answer help a serious user make progress?

