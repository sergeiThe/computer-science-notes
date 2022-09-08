# In-order

**Topic**: #algorithms 
**Relevant topics**:  #datastructures 
**Additional tags**: #flashcards
**Description**: Traversing a tree: left - self - right. [[Depth-first]]. [[Stack]].


## Demonstration

![[Pasted image 20220906084525.png]]


## Pseudocode

```
inorder(node)
	if node == null then return
	inorder(node.left)
	visit(node)
	inorder(node.right)
```


## Time complexity

O(n) - where n is the number of nodes


## Other traversal methods

- [[Pre-order]]
- [[Post-order]]
- [[Level-order]]

## Questions

- Question one: Answer (Add colon)
- Question two: Answer
