# Question 1: Subarray Sum Equals K

## Explanation

You are given an integer array and a target value `K`. Your task is to count how many contiguous subarrays have a sum exactly equal to `K`.

A subarray must contain consecutive elements from the original array. You can choose any starting and ending position as long as all elements between them are included.

For example, in `[1, 2, 1, 1, 1]` with `K = 3`, the subarrays `[1, 2]`, `[2, 1]`, and `[1, 1, 1]` each have a sum of `3`, so the answer is `3`.

The array can also contain negative values, so the sum of a subarray is not necessarily increasing as more elements are included.

## Problem Statement

You are given an integer array of length `n` and an integer `K`.

Count the number of contiguous subarrays whose sum is exactly `K`.

A subarray must contain consecutive elements from the original array.

## Input Format

The first line contains two integers `n` and `K`.

The second line contains `n` space-separated integers.

## Output Format

Print the number of contiguous subarrays whose sum is exactly `K`.

## Constraints

- `1 <= n <= 2 * 10^5`
- `-10^9 <= a[i] <= 10^9`
- `-10^14 <= K <= 10^14`

## Examples

### Example 1
**Input:**
```text
5 3
1 2 1 1 1
```
**Output:**
```text
3
```
**Explanation:** There are three contiguous subarrays that sum to 3: `[1, 2]` at indices 0-1, `[2, 1]` at indices 1-2, and `[1, 1, 1]` at indices 2-4.

### Example 2
**Input:**
```text
3 0
1 -1 0
```
**Output:**
```text
3
```
**Explanation:** The subarrays that sum to 0 are `[1, -1]` at indices 0-1, `[1, -1, 0]` at indices 0-2, and `[0]` at index 2.

## Topics

- Arrays
- Hashing
- Prefix Sum
