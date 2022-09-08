# Post-order

**Topic**: #algorithms 
**Relevant topics**:  #datastructures 
**Additional tags**: #flashcards
**Description**: Left - Right - Self. [[Depth first]]. [[Stack]]


## Demonstration

![[Pasted image 20220906085612.png]]


## Pseudocode

```

	postorder(node)
		if node == null then return
		postorder(node.left)
		postorder(node.right)
		visit(node)
	
```


## Time complexity

O(n) - where n is the number of nodes


## Questions

- Question one: Answer (Add colon)
- Question two: Answer

## Other notes

- [[Pre-order]]
- [[In-order]]
- [[Level-order]]