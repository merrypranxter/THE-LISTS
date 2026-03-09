# Vocabulary Entries Schema

This document describes the YAML format and structure for vocabulary entries used in our project.

## Structure
Each vocabulary entry follows the structure outlined below:

```yaml
entry:
  word: <string>          # The vocabulary word
  definition: <string>   # The definition of the word
  part_of_speech: <string># The part of speech (e.g., noun, verb, adjective)
  synonyms:
    - <string>           # A list of synonyms for the word
    - <string>
  antonyms:
    - <string>           # A list of antonyms for the word
    - <string>
  examples:
    - <string>           # Example sentences using the vocabulary word
    - <string>
```

## Example Entry

```yaml
entry:
  word: "benevolent"
  definition: "Well meaning and kindly."
  part_of_speech: "adjective"
  synonyms:
    - "kind"
    - "generous"
  antonyms:
    - "malevolent"
  examples:
    - "She was a benevolent ruler."
    - "His benevolent nature made him well-liked."
```

## Notes
- Ensure that every entry contains all fields for consistency.
- Use quotes for strings that include special characters or spaces.