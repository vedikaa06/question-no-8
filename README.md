# question-no-8
Solution to the question no 8 on leet code 

8. String to Integer (atoi)
Implement the myAtoi(string s) function, which converts a string to a 32-bit signed integer.

The algorithm for myAtoi(string s) is as follows:

Whitespace: Ignore any leading whitespace (" ").
Signedness: Determine the sign by checking if the next character is '-' or '+', assuming positivity if neither present.
Conversion: Read the integer by skipping leading zeros until a non-digit character is encountered or the end of the string is reached. If no digits were read, then the result is 0.
Rounding: If the integer is out of the 32-bit signed integer range [-231, 231 - 1], then round the integer to remain in the range. Specifically, integers less than -231 should be rounded to -231, and integers greater than 231 - 1 should be rounded to 231 - 1.
Return the integer as the final result.

Steps:
Skip Spaces – Ignore leading whitespaces.

Check Sign – Handle optional '+' or '-' to determine if the number is positive or negative.

Convert Digits – Read digits and build the number.

Handle Overflow – Clamp the result to stay within [-2³¹, 2³¹ − 1].
