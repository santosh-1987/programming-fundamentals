## Arrays - Prefix Sum

To fill the prefix sum array, we run through index 1 to last and keep on adding the present element with the previous
value in the prefix sum array.

| input numbers   |1|2| 3| 4| 5| 6 |...| 
|-----------------|-------| -------| -------|-------|-------|-------| -------| 
| **prefix sums** | 1 |3 |6 |10 | 15| 21 | ... |

```text
ps[0]=a[0]
ps[1]=a[0]+a[1]
ps[2]=a[0]+a[1]+a[2]
```

**OR**

```text
ps[0]=a[0]
ps[1]=ps[0]+a[1]
ps[2]=ps[1]+a[2]
```

### Applications

- **Equilibrium index of an array:** The equilibrium index of an array is an index such that the sum of elements at
  lower indexes is equal to the sum of elements at higher indexes.
    - https://www.geeksforgeeks.org/equilibrium-index-of-an-array/
- **Find if there is a subarray with 0 sum:** Given an array of positive and negative numbers, find if there is a
  subarray (of size at least one) with 0 sum.
    - https://www.geeksforgeeks.org/find-if-there-is-a-subarray-with-0-sum/
- **Maximum subarray size, such that all subarrays of that size have sum less than k:** Given an array of n positive
  integers and a positive integer k, the task is to find the maximum subarray size such that all subarrays of that size
  have the sum of elements less than k.
    - https://www.geeksforgeeks.org/maximum-subarray-size-subarrays-size-sum-less-k/
- **Find the prime numbers which can written as sum of most consecutive primes:** Given an array of limits. For every
  limit, find the prime number which can be written as the sum of the most consecutive primes smaller than or equal to
  the limit.
    - https://www.geeksforgeeks.org/find-prime-number-can-written-sum-consecutive-primes/
- **Longest Span with same Sum in two Binary arrays:** Given two binary arrays, arr1[] and arr2[] of the same size n.
  Find the length of the longest common span (i, j) where j >= i such that arr1[i] + arr1[i+1] + … + arr1[j] = arr2[i] +
  arr2[i+1] + … + arr2[j].
    - https://www.geeksforgeeks.org/longest-span-sum-two-binary-arrays/
- **Maximum subarray sum modulo m:** Given an array of n elements and an integer m. The task is to find the maximum
  value of the sum of its subarray modulo m i.e find the sum of each subarray mod m and print the maximum value of this
  modulo operation.
    - https://www.geeksforgeeks.org/maximum-subarray-sum-modulo-m/
- **Maximum subarray size, such that all subarrays of that size have sum less than k:** Given an array of n positive
  integers and a positive integer k, the task is to find the maximum subarray size such that all subarrays of that size
  have sum of elements less than k.
    - https://www.geeksforgeeks.org/maximum-subarray-size-subarrays-size-sum-less-k/
- **Maximum occurred integer in n ranges :** Given n ranges of the form L and R, the task is to find the maximum
  occurring integer in all the ranges. If more than one such integer exits, print the smallest one.
    - https://www.geeksforgeeks.org/maximum-occurred-integer-n-ranges/
- **Minimum cost for acquiring all coins with k extra coins allowed with every coin:** You are given a list of N coins
  of different denominations. you can pay an amount equivalent to any 1 coin and can acquire that coin. In addition,
  once you have paid for a coin, we can choose at most K more coins and can acquire those for free. The task is to find
  the minimum amount required to acquire all the N coins for a given value of K.
    - https://www.geeksforgeeks.org/minimum-cost-for-acquiring-all-coins-with-k-extra-coins-allowed-with-every-coin/
- **Random number generator in arbitrary probability distribution fashion:** Given n numbers, each with some frequency
  of occurrence. Return a random number with a probability proportional to its frequency of occurrence.
    - https://www.geeksforgeeks.org/random-number-generator-in-arbitrary-probability-distribution-fashion/