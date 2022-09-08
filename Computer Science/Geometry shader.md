# Geometry shader
#shader #geometry #rendering #pipeline #stage #graphics

---
```cpp

GLenum shaderType GL_GEOMETRY_SHADER

```

The [[Shaders and the Rendering Pipeline|pipeline]] stage

- Vertex shader handles vertices, geometry shader handles [[primitives]] (groups of vertices). 
- Takes primitives then "emits" their vertices to create the given primitive, or even new primitives
- Can alter data given to it to modify given primitives, or even create new ones
- Can even alter the primitive type (points, lines, triangles, etc.)