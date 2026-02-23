Step-by-step Explanation:

Check for Empty Input:
If the list is empty, return "" right away—nothing to scan.

Assume the First String is the Prefix:
Set the prefix as the first string in the list.

Scan Horizontally Across All Strings:
For each string after the first:

Check if it starts with the current prefix.
If yes, move to the next string.
If no, chop off the last character from the prefix and check again.
Keep chopping until the prefix matches the start of the string or becomes empty.
Early Exit if Prefix is Empty:
If the prefix ever becomes "", return "" immediately—no common prefix exists.

Return the Prefix:
After checking all strings, whatever’s left in prefix is your answer.

Quick Example:
For strs = ["interview", "internet", "internal"]:

Prefix = "interview"
"internet" doesn’t start with "interview" → chop last char: "intervie" (no), "intervi" (no), ... until "inter" (yes)
"internal" starts with "inter" → done!
Final answer: "inter"
Want to see this in code or try a dry run with a custom example?
