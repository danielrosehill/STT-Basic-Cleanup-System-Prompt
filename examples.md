# Examples and Templates

Including examples in your system prompt can dramatically improve the AI's understanding of your desired output style. This component focuses on how to effectively incorporate examples into your STT cleanup system prompt.

## The Power of Examples

While detailed instructions are valuable, showing the AI exactly what you want through before/after examples provides:

1. **Clarity**: Demonstrates precisely what you consider "good" output
2. **Consistency**: Helps maintain a consistent style across multiple uses
3. **Efficiency**: Often reduces the need for verbose instructions
4. **Personalization**: Allows you to showcase your unique voice and style preferences

## Implementation Approach

The most effective way to create examples:

1. Take a raw, unpolished STT output
2. Manually edit it to your preferred style
3. Include both versions in your system prompt

## Example Format

```
Here is an example of how I'd like you to transform STT text:

BEFORE:
"so I was thinking about the project timeline and um we probably need to extend it by about two weeks because of the delays in getting the materials and you know the team has been working really hard but there's just no way to make up that time so yeah we should probably talk to the client about this and see if they're okay with the new deadline"

AFTER:
I was thinking about the project timeline. We probably need to extend it by about two weeks because of delays in getting the materials.

The team has been working really hard, but there's no way to make up that time.

We should talk to the client about this and see if they're okay with the new deadline.
```

## Multiple Examples

For even better results, consider including 2-3 examples that showcase different aspects of your preferred style:

- One example demonstrating paragraph structure
- One example showing how to handle embedded instructions
- One example illustrating heading placement

## Balancing Instructions and Examples

While examples are powerful, they work best when combined with explicit instructions. The ideal approach is to:

1. Start with clear, specific instructions
2. Follow with 1-3 carefully selected examples
3. End with any additional constraints or preferences

This combination gives the AI both the "what" (instructions) and the "how" (examples) of your desired output.

## Continuous Refinement

As you use your system prompt, you may notice aspects of the AI's output that don't quite match your preferences. When this happens, create a new example based on the AI's output, edit it to your liking, and add it to your system prompt.

This iterative process allows your system prompt to evolve and improve over time, becoming increasingly tailored to your specific needs and style preferences.