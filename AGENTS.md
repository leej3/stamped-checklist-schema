# Checklist authoring guidance

## Intent and wording

The principles state the requirements; the checklist helps a reader assess a research object against them.
Preserve the intent of each mapped principle while expressing it independently as a practical assessment question.

Distinct wording serves two purposes: it makes the app less repetitive when a principle and its questions appear together, and it gives readers a second way to understand the same idea.
Expressing the same intent in two ways can help readers resolve ambiguity.

- Ask about observable evidence, actions, or outcomes a reader can check.
- Reframe the idea from the assessor's perspective rather than simply adding "Is" or "Are" to the principle or replacing words with synonyms.
- Preserve scope, requirement strength, conditions, and applicability.
  Do not silently add obligations, omit parts of a requirement, or turn an example tool into a mandatory implementation.
- Prefer a direct yes/no question that readers can understand without reconstructing missing context.
  Split independently assessable parts when this makes the answers clearer; together they must cover the intent.
- Keep necessary technical terms.
  Distinct wording is useful only when it improves clarity; forced variation can obscure meaning.
- Read each question beside its mapped principle before finalizing it.
  Would a reader learn how to check the requirement?
  Could the question be answered yes while missing the intended practice, or no for a valid implementation?
  Revise if the wording creates either mismatch.

For example, "Code-driven provenance SHOULD be recorded programmatically" can be assessed with "Does executing the code automatically produce a record of the actions it performed?"
The question describes evidence of the practice without repeating the principle's sentence structure.

## Language and readability

Review questions and documentation from the reader's perspective before finalizing them.
Consider what the reader needs to assess and what they already know.
Prefer a clear explanation over packing the most information into the fewest words.
An extra phrase or sentence is useful when it makes the meaning easier to follow.

- Make clear who or what performs an action, what it affects, and when it applies.
  Replace abstract descriptions and strings of nouns with ordinary sentences that show these relationships.
- Keep subjects near their verbs and conditions near the actions they qualify.
  Use connecting words such as "because," "which," and "after" where they help readers follow the reasoning.
- Use familiar phrasing and precise technical terms.
  Explain unfamiliar terms where readers first need them; avoid invented labels and strained metaphors.
- Name the thing being discussed when words such as "this" or "it" could refer to more than one thing.
- Reread the result without supplying context from memory, then compare it with the source for meaning.
  Preserve conditions, exceptions, uncertainty, and the distinction between evidence and interpretation.

Use these points to diagnose unclear passages, not as mechanical rules to shorten every sentence or remove every technical term.
Limit revisions to the requested passages and the surrounding text needed for consistency.

## Maintaining the data

Preserve existing item IDs for wording changes that retain the same intent.
Keep principle mappings and MUST/SHOULD/MAY groupings accurate.
Validate the JSON against LinkML and run the cross-reference and principle-coverage checks against the declared principles version, followed by pre-commit checks.
