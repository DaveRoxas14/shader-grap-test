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

# Texture Data Types
- sampler2D
- samplerCUBE

## Packed Arrays
```
fixed4 colour1 = (0,1,1,0);
```

## Packed Matrices
```
float4x4 matrix;
float myValue = matrix._m00 | _m(ROW)(COLUMN)
```

#### Chaining
```
fixed4 colour = matrix._m00_m01_m02_m03;
fixed4 colour = matrix[0] // putting entire row of matrix into an array
```


### Shader Graph Precisions
What to select?

- Single: High precision floating point, 32 bits on desktops
	- Good for world space positions, texture coordinates, multiplication variables with high complexity such as trigonometry and mathematical expressions.
- Half: Low precision floating point, 16 bits on desktops
	- Good for vectors, object space positions, high def colours (but not strong lights)

## Color
rgba = (255, 255, 255, 255) -> in Unity
rgba = (1, 1, 1, 1) -> in code // just divide by 255

## Normals
- Defining the direction each polygon is facing
- always 90 degrees?

## Colors
- Adding Colors -> going white
- Multiplying Colors -> going black