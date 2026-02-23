Step-by-step Explanation:

Check for Empty Input:
If the list is empty, just return an empty string. No prefix to find.

Start with the First String:
Assume the whole first string is the common prefix.

Compare with Each String:
For every other string in the list, compare it character by character with the current prefix:

If they match, keep going.
If they don’t, cut the prefix up to where they matched.
If at any point the prefix becomes empty, return "" right away (since there’s no common prefix).
Return the Result:
After checking all strings, whatever is left in prefix is your answer.

How it Works (Quick Example):
For strs = ["flower", "flow", "flight"]:

Start with prefix = "flower"
Compare with "flow" → common part is "flow"
Compare with "flight" → common part is "fl"
So, the answer is "fl"
