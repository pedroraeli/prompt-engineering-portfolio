# Code Assistant Prompt Template

## Purpose
Generate, review, or debug code with proper context and requirements.

## Template

\`\`\`
Generate [language] code for [functionality].

**Requirements:**
- Input: [describe expected inputs]
- Output: [describe expected outputs]
- Constraints: [performance, memory, style guide]
- Error handling: [specify requirements]
- Comments: [inline/docstring style]
- Follow: [specific style guide like PEP 8, Airbnb, etc.]

**Example usage:**
[Provide example of how code should be used]

**Edge cases to handle:**
- [edge case 1]
- [edge case 2]
\`\`\`

## Example Usage

**Input:**
\`\`\`
Generate Python code for validating email addresses.

Requirements:
- Input: String (email address)
- Output: Boolean (True if valid, False if invalid)
- Constraints: Use regex, no external libraries
- Error handling: Return False for None or empty strings
- Comments: Docstring with examples
- Follow: PEP 8

Example usage:
is_valid_email("user@example.com")  # Returns True
is_valid_email("invalid.email")     # Returns False

Edge cases to handle:
- Multiple @ symbols
- Missing domain
- Special characters
- International domains
\`\`\`

**Output:**
\`\`\`python
import re

def is_valid_email(email):
    """
    Validate email address format using regex.
    
    Args:
        email (str): Email address to validate
        
    Returns:
        bool: True if email format is valid, False otherwise
        
    Examples:
        >>> is_valid_email("user@example.com")
        True
        >>> is_valid_email("invalid.email")
        False
    """
    if email is None or email == "":
        return False
    
    # Regex pattern for email validation
    pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
    
    return bool(re.match(pattern, email))
\`\`\`