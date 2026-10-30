# Checklist authoring guidance

## Intent and wording

The principles state the requirements; the checklist helps a reader assess a research object against them.
Preserve the intent of each mapped principle while expressing it independently as a practical assessment question.

Distinct wording serves two purposes: it makes the app less repetitive when a principle and its questions appear together, and it gives readers a second way to understand the same idea.
Agreement between these two expressions helps reduce ambiguity.
Do not normalize checklist wording to match the principles verbatim, or change a principle merely to match a checklist question.

- Ask about observable evidence, actions, or outcomes a reader can check.
- Reframe the idea from the assessor's perspective rather than simply adding "Is" or "Are" to the principle or replacing words with synonyms.
- Preserve scope, requirement strength, conditions, and applicability.
  Do not silently add obligations, omit parts of a requirement, or turn an example tool into a mandatory implementation.
- Prefer a short, direct yes/no question.
  Split independently assessable parts when this makes the answers clearer; together they must cover the intent.
- Keep necessary technical terms.
  Distinct wording is useful only when it improves clarity; forced variation can obscure meaning.
- Read each question beside its mapped principle before finalizing it.
  Would a reader learn how to check the requirement?
  Could the question be answered yes while missing the intended practice, or no for a valid implementation?
  Revise if the wording creates either mismatch.

For example, "Code-driven provenance SHOULD be recorded programmatically" can be assessed with "Does executing the code automatically produce a record of the actions it performed?"
The question describes evidence of the practice without repeating the principle's sentence structure.

## Maintaining the data

Preserve existing item IDs for wording changes that retain the same intent.
Keep principle mappings and MUST/SHOULD/MAY groupings accurate.
Validate the JSON against LinkML and run the cross-reference and principle-coverage checks against the declared principles version, followed by pre-commit checks.
