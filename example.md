Here are more examples of complicated regex patterns along with detailed explanations, formatted in Markdown:

# Complex Regex Pattern Examples
The regex pattern `(?:^|\s)` is a non-capturing group that matches either the start of a string or a whitespace character. Here's a breakdown of the components:

### Breakdown of the Pattern

- `(?: ...)`: This denotes a non-capturing group. It groups the contained pattern but does not capture it for back-references.
  
- `^`: This matches the start of a string.

- `|`: This is the logical OR operator. It allows for matching either the pattern before or after it.

- `\s`: This matches any whitespace character (spaces, tabs, line breaks).


### Example Usage
If you were to use this in a regex search for a word (e.g., "example"), the full pattern might look like this:
```regex
(?:^|\s)example
```
This would match "example" if it is at the start of the string or follows a space.

### Example Matches
- **Matches**: `"example"`, `" example"`, `"\nexample"`
- **Does Not Match**: `"text example"` (the "text" does not create a match because it does not satisfy the condition of being at the start or following whitespace).


## 1. Match a Valid URL
### Pattern
```regex
^(https?:\/\/)?(www\.)?([a-zA-Z0-9-]+)(\.[a-zA-Z]{2,})(\/[a-zA-Z0-9-._~:?#@!$&'()*+,;=]*)*$
```
### Explanation
- **^**: Asserts the start of the string.
- **(https?:\/\/)?**: Matches `http://` or `https://` optionally.
- **(www\.)?**: Matches `www.` optionally.
- **([a-zA-Z0-9-]+)**: Matches the domain name consisting of alphanumeric characters and hyphens.
- **(\.[a-zA-Z]{2,})**: Matches a dot followed by a top-level domain (TLD) with at least two letters.
- **(\/[a-zA-Z0-9-._~:?#@!$&'()*+,;=]*)***: Matches an optional path that may include various characters.
- **$**: Asserts the end of the string.

---

## 2. Match a Valid IPv4 Address
### Pattern
```regex
^((25[0-5]|(2[0-4][0-9]|[01]?[0-9][0-9]?))\.){3}(25[0-5]|(2[0-4][0-9]|[01]?[0-9][0-9]?))$
```
### Explanation
- **^**: Asserts the start of the string.
- **(25[0-5]|(2[0-4][0-9]|[01]?[0-9][0-9]?))**: Matches a number between 0 and 255.
- **\.:** Matches a literal dot.
- **{3}**: Indicates that the preceding group should appear exactly three times.
- **(25[0-5]|(2[0-4][0-9]|[01]?[0-9][0-9]?))**: Matches the last segment of the IPv4 address.
- **$**: Asserts the end of the string.

### Summary
This pattern validates IPv4 addresses, ensuring each segment is between 0 and 255.

---

## 3. Match a Valid Date (YYYY-MM-DD)
### Pattern
```regex
^(19|20)\d{2}-(0[1-9]|1[0-2])-(0[1-9]|[12][0-9]|3[01])$
```
### Explanation
- **^**: Asserts the start of the string.
- **(19|20)\d{2}**: Matches years from 1900 to 2099.
- **-**: Matches the literal hyphen.
- **(0[1-9]|1[0-2])**: Matches months from 01 to 12.
- **-**: Matches another literal hyphen.
- **(0[1-9]|[12][0-9]|3[01])**: Matches days from 01 to 31.
- **$**: Asserts the end of the string.

### Summary
This pattern validates dates in the format `YYYY-MM-DD`.

---

## 4. Match a Strong Password
### Pattern
```regex
^(?=.*[A-Z])(?=.*[a-z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{12,24}$
```
### Explanation
- **^**: Asserts the start of the string.
- **(?=.*[A-Z])**: Positive lookahead for at least one uppercase letter.
- **(?=.*[a-z])**: Positive lookahead for at least one lowercase letter.
- **(?=.*\d)**: Positive lookahead for at least one digit.
- **(?=.*[@$!%*?&])**: Positive lookahead for at least one special character.
- **[A-Za-z\d@$!%*?&]{12,24}**: Matches the password length between 12 and 24 characters.
- **$**: Asserts the end of the string.

### Summary
This regex pattern enforces strong password requirements.

---

## 5. Match a Properly Nested Parentheses
### Pattern
```regex
^(\((?:[^()]*|(?R))*\))$
```
### Explanation
- **^**: Asserts the start of the string.
- **\(**: Matches an opening parenthesis.
- **(?: ... )**: Non-capturing group for the inner pattern.
- **[^()]*:** Matches any characters except parentheses.
- **|(?R)**: Recursive call to match nested parentheses.
- **\)**: Matches a closing parenthesis.
- **$**: Asserts the end of the string.

### Summary
This pattern validates properly nested parentheses, allowing for complex nesting.

---

## 6. Match a Credit Card Number
### Pattern
```regex
^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14}|3[47][0-9]{13}|6(?:011|5[0-9]{2})[0-9]{12}|3(?:0[0-5]|[68][0-9])[0-9]{11}|7[0-9]{15})$
```
### Explanation
- **^**: Asserts the start of the string.
- **(?: ... )**: Non-capturing group for different card types.
- **4[0-9]{12}(?:[0-9]{3})?**: Matches Visa card numbers.
- **5[1-5][0-9]{14}**: Matches MasterCard numbers.
- **3[47][0-9]{13}**: Matches American Express card numbers.
- **6(?:011|5[0-9]{2})[0-9]{12}**: Matches Discover card numbers.
- **3(?:0[0-5]|[68][0-9])[0-9]{11}**: Matches JCB card numbers.
- **7[0-9]{15}**: Matches UnionPay card numbers.
- **$**: Asserts the end of the string.

### Summary
This regex pattern validates various credit card formats.

---

These examples illustrate the versatility and complexity of regex patterns for different validation and matching purposes. Feel free to explore or modify them for your specific use cases!
