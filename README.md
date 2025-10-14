# This is for my Shader Graph Udemy Course...

### WIP

# The rasterization Pipeline
- how a 3D virtual object draw to screen
	- Verticies normals uvs tangents
- Vertex Processing -> Primitive Processing -> Razterization -> Fragment Processing -> buffer -> Depyh & Color processing
- Vertex block - where data  about the 3D object comes from the shader code
	- Vertex - xyz coordinates
	- normal - vector that sits out perpendicular to a face
	- tangent - another vector that sits parallel to a face, for bump mapping
	- UV - a mapping coordinate that specifies how a texture is placed on a face.
- Fragment Block - is for coloring pixels.
- The master stack - Fragment and Vertex Block combined
