# Day42-50-days-coding-challenge

# Day 42: Validate BST & Reverse Words in a String

## 🌲 Problem 1: Validate Binary Search Tree

### ✅ Problem Statement:
Given a binary tree, determine if it's a valid Binary Search Tree (BST).

### 🧠 Approach:
- Use a helper function with `min` and `max` limits.
- At each node:
  - Value must be greater than `min` and less than `max`.
  - Recurse left with updated `max = node.val`
  - Recurse right with updated `min = node.val`

### 📘 Example:
Input: [2,1,3] → Output: `true`  
Input: [5,1,4,null,null,3,6] → Output: `false`  

### 💡 Constraints:
- 1 <= nodes <= 10⁴
- Node values range from -2³¹ to 2³¹ - 1

---

## 🔤 Problem 2: Reverse Words in a String

### ✅ Problem Statement:
Given a string `s`, reverse the order of words. Remove leading/trailing/multiple spaces.

### 🧠 Approach:
- Use `s.split()` to tokenize by spaces.
- Reverse the list using slicing: `[::-1]`
- Join with single space `" ".join(...)`

### 📘 Example:
Input: `"the sky is blue"` → Output: `"blue is sky the"`  
Input: `"  hello world  "` → Output: `"world hello"`  
Input: `"a good   example"` → Output: `"example good a"`  

### 💡 Constraints:
- 1 <= s.length <= 10⁴
- s may contain extra spaces but at least one word exists

---

## 🏁 Summary
- Validating a BST requires checking **global constraints**, not just local child comparisons.
