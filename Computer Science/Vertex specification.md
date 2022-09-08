# Vertex specification
#vertex #pipeline #graphics 

---

The [[Shaders and the Rendering Pipeline|pipeline]] stage

- Vertex is a point in space, usually defined with x, y and z coordinates.
- A primitive is a simple shade defined using one or more vertices
- Usually we use triangles, but we can also use points, lines and quads.
- Fragments are per-pixel data created from primitives
- Vertex specification: setting up the data of the vertices for the primitives we want to render.
- Done in the application itself

Uses [[VAO]]s (Vertex Array Objects) and [[VBO]]s (Vertex Buffer Objects). [[Attribute pointers]]


| Creating VAO and VBO                    | Functions                 |
| --------------------------------------- | ------------------------- |
| Generate a VAO ID                       | glGenVertexArrays         |
| Bind the VAO with that ID               | glBindVertexArray         |
| Generate a VBO ID                       | glGenBuffers              |
| Bind the VBO with that ID               | glBindBuffer              |
| Attach the vertex data to that VBO      | glBufferData              |
| Define the attribute pointer formatting | glVertexAttribPointer     |
| Enable the attribute pointer            | glEnableVertexAttribArray |
| Unbind the VAO and VBO                  | glBind...                 |


## Initializing Draw

1. Activate shader program you want to use
2. Bind VAO of object you want to draw
3. Call glDrawArrays, which initiates the rest of the pipeline