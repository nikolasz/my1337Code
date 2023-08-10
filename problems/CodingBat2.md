miss_char

Problem:
Given a non-empty string and an int n, return a new string where the char at index n has been removed. The value of n will be a valid index of a char in the original string (i.e. n will be in the range 0..len(str)-1 inclusive).


missing_char('kitten', 1) → 'ktten'
missing_char('kitten', 0) → 'itten'
missing_char('kitten', 4) → 'kittn'

Solution:

def missing_char(str, n):
  return str[:n] + str[n+1:] #slicing operation to get the chars before and after index n char

Intuition:
Use the slicing operator to get the chars before and after index n char.
Return the concatenation of the two strings.

Notes:
The slicing operator will return the chars from the start index up to, but not including, the end index.
So, str[:n] will return the chars from 0 to n-1, and str[n+1:] will return the chars from n+1 to the end of the string.
The concatenation operator is +, not ,.
The concatenation operator can only be used on strings, not ints or other data types.
The slicing operator can be used on strings, lists, and tuples.
The slicing operator can be used on strings, lists, and tuples.
Python uses 0-based indexing, so the first char in a string, list, or tuple is at index 0.