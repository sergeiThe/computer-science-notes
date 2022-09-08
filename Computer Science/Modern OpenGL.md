We need to get the function declarations and link to the functions aswell.
 
We need to access driver DLL files and retrieve functions pointers to the functions inside those libraries. To access functions, we need to use win32 API calls. 

- Windows only
- Manual code writing
- Not fun

Instead it is better to use a library. It provides all the constants and declarations of functions. Libraries just provide us with the accessing the functions. 

Libraries:
1. GLEW
2. GLAD
 
Modern OpenGL has many functions.

## Start to draw something

1. Create vertex buffer
2. Create shader

**Vertex buffer** is an array of bytes of memory. 

Issue draw call.

**Shader** is code that runs on GPU.

OpenGL is a state machine.

```
unsigned buffer;
glGenBuffers(1, &buffer);
glBindBuffer(GL_ARRAY_BUFFER, buffer);
glBufferData(GL_ARRAY_BUFFER, 6 * sizeof(float), positions, GL_STATIC_DRAW);

```




