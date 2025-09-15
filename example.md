
# Regular Expression Examples

### 1. Email Address Validation
```regex
^[\w.-]+@[\w.-]+\.[a-zA-Z]{2,}$
```
- **Explanation**: Matches a valid email format like `user@example.com`.

### 2. Phone Number Format
```regex
^\(\d{3}\)\s\d{3}-\d{4}$
```
- **Explanation**: Matches a phone number in the format `(123) 456-7890`.

### 3. URL Validation
```regex
^(https?://)?(www\.)?[\w-]+\.[a-z]{2,}(/[\w./?=&%-]*)?$
```
- **Explanation**: Matches URLs, optionally starting with `http://` or `https://`.

### 4. Date Validation (MM/DD/YYYY)
```regex
^(0[1-9]|1[0-2])/(0[1-9]|[12][0-9]|3[01])/\d{4}$
```
- **Explanation**: Matches dates in the format `MM/DD/YYYY`.

### 5. Extracting Hashtags
```regex
#\w+
```
- **Explanation**: Matches hashtags in text, such as `#example`.

### 6. Finding IP Addresses
```regex
\b(?:\d{1,3}\.){3}\d{1,3}\b
```
- **Explanation**: Matches IPv4 addresses (e.g., `192.168.1.1`).

### 7. Extracting Words
```regex
\b\w+\b
```
- **Explanation**: Matches whole words in a text, ignoring punctuation.

### 8. HTML Tag Removal
```regex
<[^>]+>
```
- **Explanation**: Matches HTML tags (e.g., `<div>`).

### 9. Matching a Specific Pattern
```regex
^(?!.*duplicate).*
```
- **Explanation**: Matches any string that does not contain the word "duplicate".

### 10. Password Validation
```regex
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$
```
- **Explanation**: Matches a password that is at least 8 characters long.

### 11. Social Security Number (SSN) Format
```regex
^\d{3}-\d{2}-\d{4}$
```
- **Explanation**: Matches a Social Security Number format like `123-45-6789`.

### 12. Extracting Numbers
```regex
\d+
```
- **Explanation**: Matches one or more digits in a string.

### 13. Matching Any Character
```regex
.
```
- **Explanation**: Matches any single character except a newline.

### 14. Word Boundary
```regex
\bword\b
```
- **Explanation**: Matches the word "word" as a whole.

### 15. Optional Character
```regex
colou?r
```
- **Explanation**: Matches both "color" and "colour".

### 16. Match a Hex Color Code
```regex
^#?([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$
```
- **Explanation**: Matches hex color codes like `#FFFFFF` or `#FFF`.

### 17. Extracting Email Addresses
```regex
[\w\.-]+@[\w\.-]+\.\w+
```
- **Explanation**: Matches email addresses within text.

### 18. Match a Credit Card Number
```regex
^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14}|3[47][0-9]{13}|6(?:011|5[0-9]{2})[0-9]{12}|3(?:0[0-5]|[68][0-9])[0-9]{11}|7[0-9]{15})$
```
- **Explanation**: Matches major credit card formats.

### 19. Match a Time Format (HH:MM)
```regex
^(0?[0-9]|1[0-9]|2[0-3]):[0-5][0-9]$
```
- **Explanation**: Matches time in the format `HH:MM`.

### 20. Validate a Username
```regex
^[a-zA-Z0-9_]{3,16}$
```
- **Explanation**: Matches usernames that are 3 to 16 characters long.

### 21. Match a Positive Integer
```regex
^[1-9]\d*$
```
- **Explanation**: Matches positive integers without leading zeros.

### 22. Match a Negative Integer
```regex
^-?[1-9]\d*$
```
- **Explanation**: Matches negative integers.

### 23. Match Any Alphanumeric Character
```regex
^\w+$
```
- **Explanation**: Matches strings that contain only alphanumeric characters and underscores.

### 24. Match a Simple Password
```regex
^[A-Za-z0-9]{6,12}$
```
- **Explanation**: Matches passwords that are 6 to 12 characters long.

### 25. Match a Floating Point Number
```regex
^[+-]?(\d*\.\d+|\d+\.\d*)$
```
- **Explanation**: Matches floating point numbers, including optional signs.

### 26. Match a Non-Negative Integer
```regex
^\d+$ 
```
- **Explanation**: Matches any non-negative integer.

### 27. Match a Sentence Ending with a Period
```regex
^.*\.$
```
- **Explanation**: Matches a complete sentence that ends with a period.

### 28. Match a Specific File Extension
```regex
^.*\.(pdf|docx|txt)$
```
- **Explanation**: Matches file names that end with `.pdf`, `.docx`, or `.txt`.

### 29. Match Repeated Words
```regex
\b(\w+)\s+\1\b
```
- **Explanation**: Matches repeated words, such as "hello hello".

### 30. Match a Valid IPv6 Address
```regex
^(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|(([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}((25[0-5]|(2[0-4]|1{0,1}[0-9]|[1-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]|[1-9]){0,1}[0-9])|([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]|[1-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]|[1-9]){0,1}[0-9]))$
```
- **Explanation**: Matches valid IPv6 addresses.

### 31. Match a Strong Password
```regex
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$
```
- **Explanation**: Matches passwords that are at least 8 characters long and contain at least one lowercase letter, one uppercase letter, one digit, and one special character.

### 32. Match a Simple HTML Tag
```regex
<([a-z][a-z0-9]*)\b[^>]*>(.*?)<\/\1>
```
- **Explanation**: Matches simple HTML tags, capturing the tag name.

### 33. Match a Floating Point Number with Optional Sign
```regex
^[+-]?([0-9]*[.])?[0-9]+$
```
- **Explanation**: Matches floating point numbers that can be positive or negative.

### 34. Match a Valid Credit Card Number (Basic)
```regex
^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14})$
```
- **Explanation**: Matches Visa or MasterCard formats.

### 35. Match a Non-Empty String
```regex
^.+$
```
- **Explanation**: Matches any non-empty string.

### 36. Match a Specific Range of Numbers
```regex
^(1[0-9]|[1-9])$ 
```
- **Explanation**: Matches numbers from 1 to 19.

### 37. Match a Simple HTML Comment
```regex
<!--(.*?)-->
```
- **Explanation**: Matches HTML comments.

