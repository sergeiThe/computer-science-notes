# Per-sample operations
#shader #rendering #pipeline #stage #graphics

The [[Shaders and the Rendering Pipeline|pipeline]] stage

---

- Series of tests run to see if the fragment should be drawn
- Most important test: Depth test. Determines if something is in front of the point being drawn.
- Color Blending: using defined operations, fragment colors are blended together with overlapping fragments. Usually used to handle transparent objects.
- Fragment data written to currently bound [[framebuffer]] (usually the default buffer)
- In the application code, the use usually defines a buffer swap here, putting the newly updated framebuffer to the front
- End of the [[Shaders and the Rendering Pipeline|pipeline]]