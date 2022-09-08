# Shader

**Topic**: #graphics
**Flashcard type**: #flashcardsgraph 
**Description**: Computer program that transforms inputs to outputs while rendering.


| Step                                | Function                                       |
| ----------------------------------- | ---------------------------------------------- |
| 1. Define a shader                  | const std::string vShaderSrc = R"(shader code) |
| 2. Create the shader type           | glCreateShader(GL_VERTEX_SHADER)               |
| 3. Transform to c-string            | vShaderSrc.c_str()                             |
| 4. Point to the shader src          | glShaderSource(vShader, 1, &vss, nullptr)      |
| 5. Compile the shader               | glCompileShader(vShader)                       |
| 6. Create a program                 | glCreateProgram()                              |
| 7. Attach the shader to the program | glAttachShader(sProgram, vShader)              |
| 8. Link the program                 | glLinkProgram(sProgram)                        |
| 9. Bind the program                 | glUseProgram(sProgram)                                               |
*Table 1 - Steps of running a shader program*



## Shader programs

```cpp
auto vertexShader = glCreateShader(GL_VERTEX_SHADER);
const GLchar* vss = vertexShaderSrc.c_str();
glShaderSource(vertexShader, 1, &vss, nullptr);
glCompileShader(vertexShader);
```

## Questions

- What is a shader?::Computer program that runs for each specific section of the [[Shaders and the Rendering Pipeline|rendering pipeline]]. 
- Where is shader stored?::[[GPU]]
- What language are shaders written in?::GLSL
- 