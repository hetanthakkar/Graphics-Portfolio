# Phong Illumination and Point Light(s) Assignment

## Description
This assignment focuses on implementing the Phong illumination model and working with point lights in a 3D graphics application. The project builds upon previous work with .obj file loading and adds sophisticated lighting effects.

## Objectives
- Display .obj objects with perspective projection
- Visualize object normals for debugging
- Implement the Phong illumination model
- Create and animate point lights
- Add interactive graphics features

## Tasks
### Task 1: .obj Object Display
- Load and display a .obj file specified through command-line arguments
- Example usage: `./prog ../../common/bunny_centered.obj`

### Task 2: Displaying Normals
- Update the fragment shader to output colors based on object normals
- Store and pass normals from the vertex shader to the fragment shader

### Task 3: Phong Illumination - Point Lights
- Implement the Phong illumination model with three components:
  - Ambient
  - Diffuse
  - Specular
- Create at least one animated point light in the scene
- Implement light attenuation over distance

### Task 4: Interactive Graphics
- Implement the following keyboard controls:
  - Tab key: Toggle between filled and wireframe mode
  - Esc key: Exit the application
  - W/S keys: Move camera forward/backward
