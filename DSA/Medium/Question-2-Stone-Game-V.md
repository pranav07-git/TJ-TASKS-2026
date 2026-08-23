# Question 2: Stone Game V

## Explanation

You are given an array of positive integers representing piles of stones. Alice starts with the entire array.

At each step, Alice divides the current segment into two non-empty contiguous parts. Let the sums of the two parts be `L` and `R`.

If `L` is smaller, Alice keeps the left part and gains `L` points. If `R` is smaller, she keeps the right part and gains `R` points. When both sums are equal, Alice can choose either part and gains that common sum.

Alice continues this process with the part she keeps until it can no longer be divided.

Your task is to determine the maximum total score Alice can obtain by making the splits in the best possible way.

## Problem Statement

You are given an array of positive integers representing piles of stones.

Alice starts with the entire array.

At each step, Alice chooses a position to divide the current array segment into two non-empty contiguous parts.

Let the sums of the two parts be `L` and `R`.

- If `L < R`, Alice keeps the left part and gains `L` points.
- If `R < L`, Alice keeps the right part and gains `R` points.
- If `L = R`, Alice may choose either part and gains `L` points.

Alice continues dividing the remaining segment until it can no longer be divided.

Determine the maximum score Alice can obtain.

## Input Format

The first line contains an integer `n`.

The second line contains `n` positive integers representing the stone values.

## Output Format

Print the maximum score Alice can obtain.

## Constraints

- `1 <= n <= 500`
- `1 <= stoneValue[i] <= 10^6`

## Examples

### Example 1
**Input:**
```text
3
6 2 3
```
**Output:**
```text
7
```
**Explanation:** Alice can first divide the array into `[6]` and `[2, 3]`. Since the right part sums to 5, which is less than 6, Alice must keep the right part `[2, 3]` and scores 5 points. Next, she divides `[2, 3]` into `[2]` and `[3]`. She keeps `[2]` and scores 2 points. The array cannot be divided further. Her total score is 5 + 2 = 7.

### Example 2
**Input:**
```text
4
1 2 3 7
```
**Output:**
```text
10
```
**Explanation:** Alice optimally divides the array to collect segments with sums 6, 3, and 1, resulting in a maximum total score of 10.

## Topics

- Arrays
- Dynamic Programming
