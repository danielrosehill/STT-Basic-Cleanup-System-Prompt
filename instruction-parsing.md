# Instruction Parsing

One of the most powerful capabilities of LLMs in STT cleanup is their ability to parse and follow instructions embedded within the dictated text itself.

## The Challenge

When dictating, users often include meta-instructions or corrections within the flow of their speech:

```
"Send an email to Tom about the project deadline. Wait, actually his name is Tim. The deadline has been moved to Friday and we need to discuss the budget implications."
```

Without instruction parsing, the AI would simply clean up this text as-is, leaving in the correction and meta-commentary.

## Enhanced System Prompt

```
The text which the user provides will contain a mixture of instructions for editing and content to be added to the text. Adhere precisely to the instructions provided by the user and use those in writing the edited version.
```

## Example Scenario

**Raw STT Input:**
```
"So I have a meeting with Tom at 4 and I'd like to prepare a general instruction. Wait, sorry his name is actually Tim and here is the text of what I'd like to go in: The marketing budget for Q2 has been wrapped up. These are what I'd like to cover."
```

**With Instruction Parsing:**
The AI would understand that:
1. The meeting is with Tim (not Tom)
2. The actual content should only include "The marketing budget for Q2 has been wrapped up. These are what I'd like to cover."
3. The rest is meta-commentary about the content

**Expected Output:**
```
The marketing budget for Q2 has been wrapped up. These are what I'd like to cover.
```

## Benefits

1. **Efficiency**: No need to restart dictation when you make a mistake
2. **Natural workflow**: Allows for a more conversational approach to content creation
3. **Self-correction**: Enables on-the-fly adjustments without manual editing
4. **Reduced post-processing**: Minimizes the need for manual cleanup

## Implementation Notes

This capability works best when combined with the basic cleanup and formatting instructions. The AI should first parse and follow any embedded instructions, then apply the standard cleanup and formatting rules to the resulting content.