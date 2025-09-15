Here’s the summary of regular expressions (regex) formatted in Markdown:

```markdown
# Summary of Regular Expressions (Regex)

**Definition:**
Regular expressions (regex) are sequences of characters that form a search pattern. They are used for string matching and manipulation in text processing, allowing users to define complex search criteria.

## Components:

1. **Literals:**
   - Match specific characters, e.g., `a`, `1`, `$`.

2. **Metacharacters:**
   - Special characters that have specific meanings:
     - `.`: Matches any character except a newline.
     - `^`: Anchors the match to the start of a string.
     - `$`: Anchors the match to the end of a string.
     - `\`: Escapes a metacharacter to match it literally.

3. **Character Classes:**
   - Defined using square brackets `[]`, e.g., `[abc]` matches 'a', 'b', or 'c'.
   - Negation can be used with `^`, e.g., `[^abc]` matches any character except 'a', 'b', or 'c'.

4. **Quantifiers:**
   - Control the number of occurrences of the preceding element:
     - `*`: Zero or more.
     - `+`: One or more.
     - `?`: Zero or one.
     - `{n}`: Exactly n times.
     - `{n,m}`: Between n and m times.

5. **Anchors:**
   - Used to specify positions in the text:
     - `^`: Start of a string.
     - `$`: End of a string.
     - `\b`: Word boundary.

6. **Groups and Ranges:**
   - Parentheses `()` create capturing groups.
   - Non-capturing groups can be created using `(?:...)`.
   - Alternation (logical OR) is represented by `|`, e.g., `(cat|dog)`.

7. **Assertions:**
   - **Lookaheads**: `(?=...)` checks for a pattern ahead.
   - **Lookbehinds**: `(?<=...)` checks for a pattern behind.
   - **Negative lookaheads**: `(?!...)` ensures a pattern does not occur ahead.
   - **Negative lookbehinds**: `(?<!...)` ensures a pattern does not occur behind.

## Usage:
- Regex is widely used in programming for tasks such as:
  - Validating input (e.g., email, phone numbers).
  - Searching and replacing substrings in text.
  - Parsing text data, such as extracting information from logs or files.

## Flags:
- Modifiers that change how regex operates:
  - `g`: Global search (find all matches).
  - `i`: Case-insensitive search.
  - `m`: Multiline mode (affects `^` and `$`).

## Examples:
- `^\d{3}-\d{2}-\d{4}$`: Matches a format like "123-45-6789" (a Social Security number).
- `^[A-Z][a-z]*$`: Matches a capitalized word.

## Conclusion
Regular expressions are powerful tools for text processing, enabling complex pattern matching and manipulation. Mastery of regex can significantly enhance efficiency in data validation, searching, and text manipulation tasks.
```

Feel free to copy and use this Markdown summary as needed!
