### 104. Maximum Depth Binary Tree (Easy)

Given the root of a binary tree, return its maximum depth.

A binary tree's maximum depth is the number of nodes along the longest path from the root node down to the farthest leaf node.

Example 1:
```
Input: root = [3,9,20,null,null,15,7]
Output: 3
```
Example 2:
```
Input: root = [1,null,2]
Output: 2
```

Constraints:

- The number of nodes in the tree is in the range 0 - 10^4.
- -100 <= Node.val <= 100

<details>
  <summary><h3>Show Hint 1</h3></summary>
  <p>Just like tree traversal and just return the maximum of left and right tree + 1 at the end.</p>
</details>

---
<details>
  <summary><h3>Pseudocode</h3></summary>
  <pre>
    maxDepth(node)
      if root is null then return 0
      maxLeft -> maxDepth(node.left)
      maxRight -> maxDepth(node.right)
      return maximum(maxLeft, maxRight) + 1
  </pre>
</details>
