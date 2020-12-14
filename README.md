# Longest Common Subsequence of two Strings

Write a function `find_lcs` that takes two strings `s1` and `s2` and returns the [longest common subsequence](https://en.m.wikipedia.org/wiki/Longest_common_subsequence_problem) of `s1` and `s2`.

The longest common subsequence is the longest sequence of characters (case sensitive) such that all of them appear in both of the string, possibly with other characters in between.

For instance:

```python
>>> find_lcs('ABAZDC', 'BACBAD')
'ABAD'
>>> find_lcs('AGGTAB', 'GXTXAYB')
'GTAB'
>>> find_lcs('aaaa', 'aa')
'aa'
```

You're allowed to ignore characters to get a longest common subsequence, but the order has to be the same.

Don't worry about performance at first. Just come up with the simplest, most naive solution, most [brutal-force search](https://en.wikipedia.org/wiki/Brute-force_search) that you can. Also come up with more test cases if you would like, and it's generally helpful to write out your algorithm either as pseudocode or in natural language before you start coding.

<em>Hint: You can start with writing a function that returns all the possible sequences of a string.

For example:

```python
>>> generate_substrings('ABCD')
['', 'A', 'B', 'AB', 'C', 'AC', 'BC', 'ABC', 'D', 'AD', 'BD', 'ABD', 'CD', 'ACD', 'BCD', 'ABCD']
>>> generate_substrings('ABA')
['', 'A', 'B', 'AB', 'A', 'AA', 'BA', 'ABA']
```

</em>
