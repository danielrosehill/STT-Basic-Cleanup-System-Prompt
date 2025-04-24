# Formatting for Internet Readability

One common issue with basic STT cleanup is that it may fix grammatical issues but still leave you with a wall of text. This component focuses on transforming that text into a format suitable for online consumption.

## Enhanced System Prompt

```
Your task is to take text provided by the user and improve it for flow and accuracy.

The text was captured using speech-to-text software. Therefore you can expect that it will contain common deficiencies of STT generated text such as pause words that were not removed and missing punctuation.

You may also be able to infer obvious typos. If you encounter these, you should remediate them. 

You should also divide the text into short paragraphs of ideally no more than 3 sentences per paragraph. The edited text that you provide should be logically organized and easy to read.

Return the edited text back to the user.
```

## Key Additions

The critical addition to the basic cleanup prompt is:

```
You should also divide the text into short paragraphs of ideally no more than 3 sentences per paragraph. The edited text that you provide should be logically organized and easy to read.
```

## Why This Matters

Research consistently shows that online readers prefer shorter paragraphs. Long blocks of text are intimidating and often skipped entirely. By instructing the AI to create shorter paragraphs:

1. **Improved readability**: Text becomes easier to scan and digest
2. **Better retention**: Readers are more likely to absorb the content
3. **Increased engagement**: Lower bounce rates and higher completion rates
4. **Platform-appropriate**: Suitable for emails, blogs, social media, and other digital formats

## When to Use

This formatting enhancement is ideal when preparing text for:

- Emails
- Blog posts
- Social media content
- Forum posts (Reddit, Discord, etc.)
- Documentation
- Any text that will be read on screens

It's particularly valuable when you want your content to be accessible and engaging without significant manual reformatting.