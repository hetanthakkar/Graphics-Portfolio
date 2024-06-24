# Textured .obj Model Renderer

## Project Description

This project implements a 3D renderer capable of loading and displaying textured .obj models with OpenGL. It features perspective projection, interactive camera controls, and the ability to toggle between filled and wireframe rendering modes.

## Features

- Loads and renders textured 3D models in .obj format
- Parses associated material (.mtl) files for texture information
- Implements perspective camera projection
- Provides interactive camera controls
- Supports wireframe and filled rendering modes
- Efficient handling of vertex and texture coordinate data

## Dependencies

- OpenGL 3.3+
- SDL2
- C++11 or higher

## Building the Project

To build the project, use the provided `build.py` script:

```
python3 build.py
```

This script handles all necessary compilation steps.

## Running the Program

After building, run the program with:

```
./prog path/to/your/model.obj
```

For example:

```
./prog "./../../common/objects/chapel/chapel_obj.obj"
```

## Controls

- `Tab`: Toggle between filled and wireframe rendering modes
- `Esc`: Exit the application
- `W`: Move camera forward
- `S`: Move camera backward

## Implementation Details

### OBJ and MTL Parsing

The project includes a custom OBJ loader class that handles:
- Vertex, texture coordinate, and face data parsing from .obj files
- Material and texture information parsing from .mtl files
- Efficient indexing of vertex and texture data for OpenGL rendering

### Rendering

- Uses modern OpenGL techniques with Vertex Buffer Objects (VBOs) and Element Buffer Objects (EBOs)
- Implements basic fragment and vertex shaders for textured rendering
- Applies perspective projection for realistic 3D visualization

### Camera System

Implements a simple camera system allowing forward and backward movement, enhancing the 3D viewing experience.

## Code Structure

- `main.cpp`: Entry point and main rendering loop
- `OBJLoader.hpp/cpp`: Classes for loading and processing .obj and .mtl files
- `Shader.hpp/cpp`: Shader loading and compilation utilities
- `Camera.hpp/cpp`: Basic camera implementation
- `vert.glsl` and `frag.glsl`: Vertex and fragment shaders

## Future Improvements

- Support for multiple textures per model
- Implementation of more advanced shading techniques
- Addition of dynamic lighting

## Resources Used

- [OpenGL Documentation](https://docs.gl/)
- [SDL2 API Wiki](https://wiki.libsdl.org/)
- [LearnOpenGL](https://learnopengl.com/)

## Acknowledgments

This project was completed as part of a computer graphics course, building on concepts of 3D rendering, file parsing, and interactive graphics.
