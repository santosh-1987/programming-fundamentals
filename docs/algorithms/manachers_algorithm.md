## Manacher’s Algorithm – Linear Time Longest Palindromic Substring 
Given a string, find the longest substring which is palindrome.

### Statement
Given string  with length . Find all the pairs  such that substring  is a palindrome. String  is a palindrome when  ( is a reversed string for ).
### More precise statement
In the worst case string might have up to  palindromic substrings, and at the first glance it seems that there is no linear algorithm for this problem.

But the information about the palindromes can be kept in a compact way: for each position  we will find the number of non-empty palindromes centered at this position.

Palindromes with a common center form a contiguous chain, that is if we have a palindrome of length  centered in , we also have palindromes of lengths ,  and so on also centered in . Therefore, we will collect the information about all palindromic substrings in this way.

Palindromes of odd and even lengths are accounted for separately as  and . For the palindromes of even length we assume that they're centered in the position  if their two central characters are  and .


### References:
https://www.geeksforgeeks.org/manachers-algorithm-linear-time-longest-palindromic-substring-part-1/