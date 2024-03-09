llucination Cheat Sheet

## Types of Contradictions

**Sentence Contradiction:**

- **USER:** What is the {characteristic A} of the {object}?
- **SYSTEM:** The {object} has {characteristic A, value X} and {characteristic A, value Y}.

**Prompt Contradiction:**

- **USER:** Write a {characteristic, positive value} review of {object}.
- **SYSTEM:** The {object} receives a {characteristic, negative value} review.

**Factual Contradiction:**

- **USER:** Who is Barack Obama?
- **SYSTEM:** Barack Obama served as the 1st president of the USA.

**Nonsensical Contradiction:**

- **USER:** The {characteristic or attribute X} of {object C}.
- **SYSTEM:** The {characteristic or attribute X} of {object C} is {Z}, and the {characteristic or attribute X} of {object D} is also {Z}.

## Causes of Contradictions

**Data Quality:**

- Noises
- Errors
- Biases
- Inconsistencies

**Generation Method:**

- May introduce biases.
- Balances between factors like:
    - Fluency and diversity
    - Accuracy and novelty

**Input Context:**

- Prioritizes given context information, even if it contains misinformation or inconsistencies.

## Minimization Strategies

**Clear Specific Prompts:**

- The more precise and detailed the input prompt, the more likely the LLM generates relevant and accurate outputs.
- Helps the model understand the expected information in the response.

**Active Mitigations:**

- Adjust Temperature:
    - Lower temperatures generate conservative and focused responses.
    - Higher temperatures generate diverse and creative responses.

**Multi-shot Prompting:**

- Provides the LLM with multiple examples of the desired output format and/or context.
- Primes the model for a clearer understanding of user expectations.
