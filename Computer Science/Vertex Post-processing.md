# Vertex post-processing
#shader #vertex #rendering #pipeline #stage #postprocessing #graphics

---

The [[Shaders and the Rendering Pipeline|pipeline]] stage

**Transform feedback** (if enabled):
- Result of vertex and geometry stages saved to [[buffer|buffers]] for later use

**Clipping**:
- [[Primitives]] that won't be visible are removed (we don't want to draw things we can't see!)
- Positions converted from "clip-space" to "window space"