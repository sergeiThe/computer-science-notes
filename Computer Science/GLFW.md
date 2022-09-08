# GLFW

**Topic**: #graphics 
**Relevant topics**:  #rendering 
**Additional tags**: #flashcardsgraph
**Description**: 

| Steps                                       | Functions                                |
| ------------------------------------------- | ---------------------------------------- |
| Init library                                | glfwInit()                               |
| Create windowed mode window and its context | glfwCreateWindow()                        |
| Make the window's context current           | glfwMakeContextCurrent()                 |
| Game loop                                   | while(!glfwWindowShouldClose(window))... |
| Close library                               | glfwTerminate()                                         |
*Table 1. GLFW steps*

## Setting up a window and OpenGL context

```cpp
#include <GLFW/glfw3.h>

int main(void)
{
    GLFWwindow* window;

    /* Initialize the library */
    if (!glfwInit())
        return -1;

    /* Create a windowed mode window and its OpenGL context */
    window = glfwCreateWindow(640, 480, "Hello World", NULL, NULL);
    if (!window)
    {
        glfwTerminate();
        return -1;
    }

    /* Make the window's context current */
    glfwMakeContextCurrent(window);

    /* Loop until the user closes the window */
    while (!glfwWindowShouldClose(window))
    {
        /* Render here */
        glClear(GL_COLOR_BUFFER_BIT);

        /* Swap front and back buffers */
        glfwSwapBuffers(window);

        /* Poll for and process events */
        glfwPollEvents();
    }

    glfwTerminate();
    return 0;
}
```




## Questions

- Question one: Answer (Add colon)
- Question two: Answer
