# Question 2: Second Largest Distinct Element

## Explanation

You are given an array of integers and need to find its second largest distinct value.

The word **distinct** is important here. If a value appears multiple times, it is still counted only once.

For example, in `[10, 5, 20, 20, 8, 10, 15]`, the distinct values are `10, 5, 20, 8, 15`. The largest is `20`, so the second largest distinct value is `15`.

If the array contains fewer than two distinct values, there is no second largest distinct value, so the answer is `-1`.

## Problem Statement

You are given an array of `n` integers.

Find the second largest DISTINCT value in the array.

If the array contains fewer than two distinct values, print `-1`.

## Input Format

The first line contains an integer `n`.

The second line contains `n` space-separated integers.

## Output Format

Print the second largest distinct value.
If it does not exist, print `-1`.

## Constraints

- `2 <= n <= 2 * 10^5`
- `-10^9 <= a[i] <= 10^9`

## Examples

### Example 1
**Input:**
```text
7
10 5 20 20 8 10 15
```
**Output:**
```text
15
```
**Explanation:** The distinct elements are 5, 8, 10, 15, and 20. The largest is 20, and the second largest is 15.

### Example 2
**Input:**
```text
5
7 7 7 7 7
```
**Output:**
```text
-1
```
**Explanation:** There is only one distinct element (7), so a second largest distinct element does not exist.

### Example 3
**Input:**
```text
6
-5 -2 -10 -2 -7 -1
```
**Output:**
```text
-2
```
**Explanation:** The distinct elements are -10, -7, -5, -2, and -1. The largest is -1, and the second largest is -2.

## Topics

- Arrays
