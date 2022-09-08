# Shaders and rendering pipeline
#shader #vertex #rendering #pipeline #graphics

The rendering pipeline is a series of stages for rendering an image to the screen. Shaders are piece of code written in GLSL which is based on C. The process of transforming 3D coordinates to 2D pixels is managed by the graphics pipeline of OpenGL. 

The graphics pipeline can be divided into two large parts: the first transforms your 3D coordinates into 2D coordinates and the second part transforms the 2D coordinates into actual colored pixels.

The processing cores run small programs on the GPU for each step of the pipeline. These small programs are called shaders.

---

1. [[Vertex specification]]
2. [[Vertex shader]] - programmable, mandatory
3. [[Tessellation]] - programmable
4. [[Geometry shader]] - programmable
5. [[Vertex Post-processing]]
6. [[Primitive Assembly]]
7. [[Rasterization]]
8. [[Fragment shader]] - programmable
9. [[Per-sample operations]]

![[pipelinevisual.png]]





## Other notes

- [[VAO]]
- [[VBO]]
- [[Shader]]
- [[Rendering loop]]
- [[GLFW]]
- [[GLAD]]