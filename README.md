# Normal Mapped OBJ Model Renderer

This project implements a renderer for 3D models in OBJ format with normal mapping support. It uses OpenGL for rendering and SDL2 for window management and input handling.

## Features

- Loads and renders OBJ format 3D models
- Supports normal mapping for enhanced surface detail
- Interactive camera controls
- Wireframe rendering mode
- Perspective projection

## Dependencies

- OpenGL 3.3+
- SDL2
- GLM (OpenGL Mathematics)

## Building

To build the project, use the provided `build.py` script:

```bash
python3 build.py
```

## Usage

Run the program with the path to an OBJ file as an argument:

```bash
./prog "./path/to/your/model.obj"
```

## Controls

- `W`: Toggle wireframe mode
- `Q`: Quit the application
- Mouse: Rotate the camera

## Implementation Details

The project is structured around several key components:

1. **OBJ Loader**: Parses OBJ files and associated material files to load geometry, texture coordinates, and normal data.
2. **Shader Management**: Implements vertex and fragment shaders for normal mapping.
3. **Texture Handling**: Loads and applies diffuse and normal map textures.
4. **Rendering Loop**: Manages the main rendering loop, including user input and OpenGL draw calls.

## Future Improvements

- Support for multiple models and textures
- Dynamic lighting
- Performance optimizations for large models

## Screenshot

![Screenshot](./NormalMap.gif)
