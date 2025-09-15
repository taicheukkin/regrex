
# MCQ Questions on Regular Expressions

1. **What does the regex `^abc` match?**
   - A) Any string containing "abc"
   - B) Strings starting with "abc"
   - C) Strings ending with "abc"
   - D) None of the above  
   **Answer:** B

2. **What does the regex `\d` represent?**
   - A) Any digit character
   - B) Any non-digit character
   - C) Any whitespace character
   - D) Any alphanumeric character  
   **Answer:** A

3. **Which regex matches an email address?**
   - A) `\w+@\w+\.\w+`
   - B) `\d+@\d+\.\d+`
   - C) `\s+@\s+\.\s+`
   - D) `@[\w.]+`  
   **Answer:** A

4. **What does `a*` mean in regex?**
   - A) Match 'a' once or more
   - B) Match 'a' zero or more times
   - C) Match 'a' exactly
   - D) Match 'a' or 'A'  
   **Answer:** B

5. **Which of the following regex matches any character?**
   - A) `.`
   - B) `*`
   - C) `?`
   - D) `+`  
   **Answer:** A

6. **What does `\w{3}` match?**
   - A) Any three words
   - B) Three digit characters
   - C) Three alphanumeric characters
   - D) Three whitespace characters  
   **Answer:** C

7. **What does `[^abc]` match?**
   - A) Any character except 'a', 'b', or 'c'
   - B) Only 'a', 'b', or 'c'
   - C) Any digit
   - D) Any whitespace  
   **Answer:** A

8. **Which regex matches a space?**
   - A) `\s`
   - B) `\d`
   - C) `\w`
   - D) `\b`  
   **Answer:** A

9. **What does `a{2,4}` mean?**
   - A) Match 'a' exactly twice
   - B) Match 'a' between 2 and 4 times
   - C) Match 'a' at least 2 times
   - D) Match 'a' at most 4 times  
   **Answer:** B

10. **What does `\bword\b` signify?**
    - A) The word "word" anywhere in a string
    - B) The exact word "word" at the boundary
    - C) The word "word" followed by a digit
    - D) The word "word" followed by a space  
    **Answer:** B

11. **Which regex matches a string that starts with a digit?**
    - A) `^\d`
    - B) `\d$`
    - C) `\d*`
    - D) `\d+`  
    **Answer:** A

12. **What does `x|y` do in regex?**
    - A) Matches either 'x' or 'y'
    - B) Matches 'xy'
    - C) Matches 'yx'
    - D) None of the above  
    **Answer:** A

13. **What does the regex `(?i)abc` do?**
    - A) Matches "abc" in lowercase only
    - B) Matches "ABC" in uppercase only
    - C) Matches "abc" case-insensitively
    - D) Matches "abc" with special characters  
    **Answer:** C

14. **Which regex matches a URL?**
    - A) `https?://[^\s]+`
    - B) `\w+@\w+\.\w+`
    - C) `\d+.\d+`
    - D) `\s+`  
    **Answer:** A

15. **What does `+` signify in regex?**
    - A) One or more occurrences
    - B) Zero or more occurrences
    - C) Exactly one occurrence
    - D) None of the above  
    **Answer:** A

16. **What is the function of `^` in regex?**
    - A) Denotes the end of a string
    - B) Denotes the start of a string
    - C) Denotes a special character
    - D) None of the above  
    **Answer:** B

17. **Which regex matches a hex color code?**
    - A) `#?[A-Fa-f0-9]{6}`
    - B) `#\d{6}`
    - C) `\w{6}`
    - D) `#\w{6}`  
    **Answer:** A

18. **What does `\d{2,4}` match?**
    - A) Exactly 2 digits
    - B) At least 2 but not more than 4 digits
    - C) Exactly 4 digits
    - D) Any number of digits  
    **Answer:** B

19. **What does `.*` match?**
    - A) Any string including empty
    - B) Any character followed by a space
    - C) Any string without spaces
    - D) None of the above  
    **Answer:** A

20. **What does the regex `\A` signify?**
    - A) Start of the string
    - B) End of the string
    - C) A whitespace character
    - D) A digit character  
    **Answer:** A

21. **What does `$` indicate in regex?**
    - A) Start of a string
    - B) End of a string
    - C) A digit
    - D) None of the above  
    **Answer:** B

22. **Which regex matches a valid phone number?**
    - A) `\d{3}-\d{3}-\d{4}`
    - B) `\(\d{3}\)\s\d{3}-\d{4}`
    - C) `\d{10}`
    - D) All of the above  
    **Answer:** D

23. **What does `(?=abc)` signify?**
    - A) Positive lookahead for "abc"
    - B) Negative lookahead for "abc"
    - C) Positive lookbehind for "abc"
    - D) Matches "abc"  
    **Answer:** A

24. **What does `(?<!abc)` signify?**
    - A) Positive lookbehind for "abc"
    - B) Positive lookahead for "abc"
    - C) Negative lookbehind for "abc"
    - D) Matches "abc"  
    **Answer:** C

25. **Which regex will find a word boundary?**
    - A) `\b`
    - B) `\B`
    - C) `^`
    - D) `$`  
    **Answer:** A

26. **What does `a{1,}` mean?**
    - A) At least one 'a'
    - B) At most one 'a'
    - C) Exactly one 'a'
    - D) Zero or more 'a's  
    **Answer:** A

27. **Which regex matches a date in the format MM/DD/YYYY?**
    - A) `\d{2}/\d{2}/\d{4}`
    - B) `\d{2}-\d{2}-\d{4}`
    - C) `\d{2}\.\d{2}\.\d{4}`
    - D) All of the above  
    **Answer:** A

28. **What does `\p{L}` match?**
    - A) Any letter
    - B) Any digit
    - C) Any whitespace
    - D) Any punctuation  
    **Answer:** A

29. **What does `\S` represent?**
    - A) Any non-whitespace character
    - B) Any whitespace character
    - C) Any digit
    - D) Any letter  
    **Answer:** A

30. **Which regex matches a string containing 'cat' but not as a whole word?**
    - A) `cat`
    - B) `\bcat\b`
    - C) `\w*cat\w*`
    - D) `cat\w*`  
    **Answer:** C

31. **What is the purpose of the escape character `\`?**
    - A) To denote a special character
    - B) To match the preceding character literally
    - C) To indicate a character class
    - D) Both A and B  
    **Answer:** D

32. **Which regex will match a string containing only vowels?**
    - A) `[aeiou]+`
    - B) `[^aeiou]+`
    - C) `\w+`
    - D) `\d+`  
    **Answer:** A

33. **What does `{n}` signify in regex?**
    - A) At least n occurrences
    - B) Exactly n occurrences
    - C) At most n occurrences
    - D) None of the above  
    **Answer:** B

34. **Which regex matches a string that starts with "Hello" and ends with "World"?**
    - A) `^Hello.*World$`
    - B) `Hello.*World`
    - C) `.*Hello.*World.*`
    - D) `Hello.*World^`  
    **Answer:** A

35. **What does `(?:...)` do in regex?**
    - A) Creates a capturing group
    - B) Creates a non-capturing group
    - C) Matches a literal string
    - D) None of the above  
    **Answer:** B

36. **Which regex will match a string containing exactly four digits?**
    - A) `\d{4}`
    - B) `\d{4,}`
    - C) `\d+`
    - D) `\w{4}`  
    **Answer:** A

37. **What does `\W` match?**
    - A) Any non-word character
    - B) Any word character
    - C) Any digit
    - D) Any whitespace character  
    **Answer:** A

38. **Which regex will match a valid IPv4 address?**
    - A) `\d{1,3}(\.\d{1,3}){3}`
    - B) `(\d{1,3}.){3}\d{1,3}`
    - C) `\d{3}.\d{3}.\d{3}.\d{3}`
    - D) `(\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})`  
    **Answer:** A

39. **What does `\b` denote in regex?**
    - A) Start of a word
    - B) End of a word
    - C) Word boundary
    - D) Both A and B  
    **Answer:** C

40. **What is the purpose of the `g` flag in regex?**
    - A) To search globally in the string
    - B) To make the search case-insensitive
    - C) To match only the first occurrence
    - D) None of the above  
    **Answer:** A

41. **What does `(?<=abc)` do?**
    - A) Matches 'abc' before the current position
    - B) Matches 'abc' after the current position
    - C) Matches 'abc' as a whole word
    - D) None of the above  
    **Answer:** A

42. **Which regex matches a string containing at least one uppercase letter?**
    - A) `[A-Z]+`
    - B) `[a-z]+`
    - C) `[0-9]+`
    - D) `\w+`  
    **Answer:** A

43. **What does `\d{4}-\d{2}-\d{2}` match?**
    - A) A date in the format YYYY-MM-DD
    - B) A time in the format HH-MM-SS
    - C) A string of digits
    - D) None of the above  
    **Answer:** A

44. **Which regex matches a string with only letters and digits?**
    - A) `^[\w]+$`
    - B) `^[a-zA-Z]+$`
    - C) `^\d+$`
    - D) Both A and B  
    **Answer:** D

45. **What does `*?` do in regex?**
    - A) Matches zero or more occurrences lazily
    - B) Matches zero or more occurrences greedily
    - C) Matches exactly one occurrence
    - D) None of the above  
    **Answer:** A

46. **Which regex matches a string containing any three characters followed by "xyz"?**
    - A) `.{3}xyz`
    - B) `xyz.{3}`
    - C) `.{3,}xyz`
    - D) `xyz.{3,}`  
    **Answer:** A

47. **What does `\d{1,2}` match?**
    - A) One or two digits
    - B) Exactly two digits
    - C) At least one digit
    - D) None of the above  
    **Answer:** A

48. **Which regex will match a string that contains "hello" anywhere?**
    - A) `^hello$`
    - B) `hello`
    - C) `.*hello.*`
    - D) Both B and C  
    **Answer:** D

49. **What does `\s+` signify?**
    - A) One or more whitespace characters
    - B) Zero or more whitespace characters
    - C) A single whitespace character
    - D) None of the above  
    **Answer:** A

50. **Which regex matches a valid credit card number?**
    - A) `\d{4}-\d{4}-\d{4}-\d{4}`
    - B) `\d{16}`
    - C) `(\d{4}-){3}\d{4}`
    - D) All of the above  
    **Answer:** D

51. **What does `(?<!a)` signify?**
    - A) Positive lookbehind for 'a'
    - B) Negative lookbehind for 'a'
    - C) Matches 'a' as a whole word
    - D) None of the above  
    **Answer:** B

52. **Which regex matches a string that contains an optional "s" at the end?**
    - A) `s?`
    - B) `s*`
    - C) `s+`
    - D) `s{0,1}`  
    **Answer:** A

53. **What does `[a-zA-Z]{5}` match?**
    - A) Exactly five letters
    - B) At least five letters
    - C) Exactly five digits
    - D) None of the above  
    **Answer:** A

54. **Which regex matches a string that contains "cat" not followed by "s"?**
    - A) `cat(?!s)`
    - B) `cat`
    - C) `cat$`
    - D) `^cat`  
    **Answer:** A

55. **What does `\d{2}:\d{2}` match?**
    - A) A time in the format HH:MM
    - B) A duration in minutes and seconds
    - C) A string of digits
    - D) None of the above  
    **Answer:** A

56. **Which regex matches a non-capturing group?**
    - A) `(?:...)`
    - B) `(...)`
    - C) `[abc]`
    - D) `\w`  
    **Answer:** A

57. **What does `\1` represent in regex?**
    - A) The first capturing group
    - B) The first digit
    - C) The first letter
    - D) None of the above  
    **Answer:** A

58. **Which regex matches a string that contains "foo" followed by zero or more "bar"?**
    - A) `foo(bar)*`
    - B) `foo(bar)+`
    - C) `foo(bar)?`
    - D) `foo(bar{0,})`  
    **Answer:** A

59. **What does `(?<=\d)` signify?**
    - A) Positive lookbehind for a digit
    - B) Positive lookahead for a digit
    - C) Negative lookbehind for a digit
    - D) None of the above  
    **Answer:** A

60. **Which regex matches a string that starts and ends with the same character?**
    - A) `^(.)\1$`
    - B) `^(.).*\1$`
    - C) `^(.)(.*)\1$`
    - D) All of the above  
    **Answer:** D

61. **What does `(?i)` do in regex?**
    - A) Makes the regex case-sensitive
    - B) Makes the regex case-insensitive
    - C) Matches only uppercase letters
    - D) None of the above  
    **Answer:** B

62. **Which regex matches a string containing only digits?**
    - A) `^\d+$`
    - B) `^\D+$`
    - C) `^\w+$`
    - D) `^[A-Z]+$`  
    **Answer:** A

63. **What does `{n,m}` signify in regex?**
    - A) At least n and at most m occurrences
    - B) Exactly n occurrences
    - C) At most n occurrences
    - D) None of the above  
    **Answer:** A

64. **Which regex matches a string with an even number of digits?**
    - A) `^\d{2}*$`
    - B) `^\d{2}(?:\d{2})*$`
    - C) `^\d{1,2}*$`
    - D) None of the above  
    **Answer:** B

65. **What does `\D` match?**
    - A) Any non-digit character
    - B) Any digit character
    - C) Any whitespace character
    - D)
