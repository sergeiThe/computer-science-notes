# VBO

**Topic**: #graphics 
**Relevant topics**: #shader #vertexshader   
**Additional tags**: #flashcardsgraph 
**Description**: Source for vertex array data. GPU

Vertex data can be more than just vertex positions.
- Color
- Normals
- Texture coordinates

## How are they generated?

```cpp
GLuint vbos;
glGenBuffers(4, &vbos);
glDelBuffers(4, &vbos);

```


## Creation and Data Transfer

![[Pasted image 20220908161954.png]]
## Linking vertex attributes

![[Pasted image 20220908161815.png]]




## Questions

What is VBO?::GPU memory area for vertex data.
What does VBO do?::Stores the vertex data defined by [[VAO]]