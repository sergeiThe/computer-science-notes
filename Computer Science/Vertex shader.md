# Vertex shader

**Topic**: #graphics 
**Relevant topics**:  #vertex #shader #vertexshader
**Additional tags**: #flashcards
**Description**: Vertex shaders process individual vertices



```cpp

GLenum shaderType GL_VERTEX_SHADER

```


```cpp
static const char* vShader = "                          \n\
	#version 330                                         \n\
				                                          \n\
	layout (location = 0) in vec3 pos;                     \n\
	void main()                                             \n\
		{                                                    \n\
    gl_Position = vec4(0.4 * pos.x, 0.4 * pos.y, pos.z, 1.0); \n\
}";
```



- Handles vertices individually
- NOT optional
- Must store something in gl_Position as it used by later stages
- Can specify additional outputs that can be picked up and used by user-defined shaders later in pipeline.
- Inputs consist of the vertex data itself
- Executed once per vertex on the GPU


## Other notes

- [[Fragment shader]]
- [[Shaders and the Rendering Pipeline]]



