# Fragment shader

**Topic**: #graphics 
**Relevant topics**:  #shader #fragment #pipeline #rendering #stage 
**Additional tags**: #flashcardsgraph 
**Description**: All about calculating the color output of our pixels. 

```cpp

GLenum shaderType GL_FRAGMENT_SHADER

```

## Sample code

```cpp
static const char* fShader = "                   \n\
#version 330                                     \n\
				                                 \n\
out vec4 colour;                                 \n\
layout (location = 0) in vec3 pos;               \n\
void main()                                      \n\
{                                                \n\
    colour = vec4(0.4, 0.4, 0.0, 1.0);           \n\
}";
```

- Handles data for each fragment
- Is optional but it's rare to not use it. Exceptions are cases where only depth or stencil data is required
- Most importand output is the color of the pixel that the fragment covers
- Simplest OpenGL programs usually have a [[Vertex shader|vertex shader]] and a fragment shader


## Other notes

- [[Vertex shader]]
- [[Shaders and the Rendering Pipeline]]