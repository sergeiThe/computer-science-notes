# Pre-order

**Topic**: #algorithms 
**Relevant topics**:  #datastructures 
**Additional tags**: #flashcards
**Description**: Traversing a tree: self - left - right. [[Depth-first]]. [[Stack]].


## Demonstration

![[Pasted image 20220906084021.png]]

## Pseudocode
```
preorder(node)
	if node == null then return
	visit(node)
	preorder(node.left)
	preorder(node.right)
	
```

## Time complexity

O(n) - where n is the number of nodes


## Other traversal methods

- [[In-order]]
- [[Post-order]]
- [[Level-order]]

## Questions

