# Question 1: Balanced Brackets

## Explanation

You are given a string containing three types of brackets: `()`, `[]`, and `{}`.

The brackets are balanced when every opening bracket has a matching closing bracket and the brackets are closed in the correct order.

For example, `{[()]}` is balanced because each opening bracket is closed by its matching bracket in the correct order.

However, `{[(])}` is not balanced because the brackets are closed in the wrong order.

Your task is to determine whether the given string is balanced.

## Problem Statement

You are given a string `s` containing only the following bracket characters:

`(` `)` `[` `]` `{` `}`

Determine whether the brackets in the string are balanced.

A string is considered balanced if:

1. Every opening bracket has a corresponding closing bracket.
2. Brackets are closed in the correct order.
3. No closing bracket appears without its corresponding opening bracket.

## Input Format

A single string `s`.

## Output Format

Print `YES` if the string is balanced.
Otherwise, print `NO`.

## Constraints

- `1 <= |s| <= 2 * 10^5`

## Examples

### Example 1
**Input:**
```text
{[()]}
```
**Output:**
```text
YES
```
**Explanation:** The brackets are correctly nested and closed in the reverse order they were opened.

### Example 2
**Input:**
```text
{[(])}
```
**Output:**
```text
NO
```
**Explanation:** The square bracket `[` is incorrectly closed by `)` instead of `]`.

### Example 3
**Input:**
```text
((()))
```
**Output:**
```text
YES
```
**Explanation:** All parentheses are matched correctly.

### Example 4
**Input:**
```text
([)]
```
**Output:**
```text
NO
```
**Explanation:** The bracket `(` is incorrectly closed by `]` instead of `)`.

## Topics

- Stack
- Strings
