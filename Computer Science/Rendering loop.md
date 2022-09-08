# Rendering loop

**Topic**: #graphics 
**Relevant topics**:  #rendering 
**Additional tags**: #flashcardsgraph 
**Description**: 



```cpp
while(true)
{
	glClear(GL_COLOR_BUFFER_BIT);


	glBindVertexArray(VAO);
	glUseProgram(shader);

	glDrawArrays(GL_TRIANGLES,  // Primitive type
				0,              // First element in buffer
				3);             // Number of elements to render

	glfwSwapBuffers(window);
}
```




## Questions

- Question one: Answer (Add colon)
- Question two: Answer
