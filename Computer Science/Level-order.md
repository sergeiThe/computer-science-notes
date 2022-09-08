# Level-order

**Topic**: #algorithms 
**Relevant topics**:  #datastructures 
**Info sources**: https://www.youtube.com/watch?v=IozGo2kwRYE&ab_channel=MichaelSambol
**Additional tags**: #flashcards
**Description**: [[Breadth-first]]. [[Queue]]. 



## Demonstration

![[Pasted image 20220906090546.png]]


## Pseudocode

```

	levelorder(root)
		q = empty queue
		q.enqueue(root)
		while(!q.isEmpty())
			node = q.dequeue()
			visit(node)
			if (node.left != null)
				q.enqueue(node.left)
			if(node.right != null)
				q.enqueue(node.right)
				
```


## Time complexity

O(n) - n is the number of nodes


## Questions

- Question one: Answer (Add colon)
- Question two: Answer


