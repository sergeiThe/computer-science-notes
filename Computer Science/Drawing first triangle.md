# First triangle (legacy opengl)
```cpp


        glClear(GL_COLOR_BUFFER_BIT);

        glBegin(GL_TRIANGLES);
        glVertex2f(-0.5f, -0.5f);
        glVertex2f(0.0f, 0.5f);
        glVertex2f(0.5f, -0.5f);

        glEnd();


        /* Swap front and back buffers */
        glfwSwapBuffers(window);
        
```



