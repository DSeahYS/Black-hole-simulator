# Black Hole Simulation

A computational astrophysics project for simulating and visualizing black holes using C++ and OpenGL.

## Project Overview

This project implements a real-time black hole simulation, starting with the Schwarzschild metric (non-rotating black hole) and with plans to extend to the Kerr metric (rotating black holes). The simulation uses GPU-accelerated ray tracing to visualize gravitational lensing, accretion disks, and spacetime curvature effects.

**Current Status: Work in Progress / On Hold**

The project is currently incomplete and not fully functional. It provides a basic framework for black hole visualization but requires significant development to achieve accurate physics simulation. Development has been paused indefinitely.

## Features (Implemented and Planned)

### Current Implementation
- Basic Schwarzschild black hole geometry
- GPU-accelerated geodesic ray tracing
- Gravitational lensing visualization
- OpenGL-based rendering

### Planned Enhancements (Not Implemented)
- Upgrade to Kerr metric for rotating black holes
- Physically accurate Novikov-Thorne accretion disk model
- Relativistic Doppler beaming and gravitational redshift
- Ergosphere visualization
- Real-time interactive simulation

## Project Structure

- `source/`: Main C++ source code and shaders
  - `black_hole.cpp`: Main application
  - `ray_tracing.cpp`: Ray tracing implementation
  - `geodesic.comp`: GPU compute shader for geodesic integration
  - `CMakeLists.txt`: Build configuration
- `Research/`: Research documentation and enhancement proposals
- `temp_extract/`: Extracted code from external sources

## Building and Running

### Requirements
- C++ compiler supporting C++17 or newer
- CMake 3.10+
- Vcpkg package manager
- Git
- OpenGL development libraries

### Build Instructions

1. Clone the repository:
   ```
   git clone https://github.com/DSeahYS/Black-hole-simulator.git
   cd Black-hole-simulator
   ```

2. Install dependencies using Vcpkg:
   ```
   vcpkg install
   ```

3. Configure the build:
   ```
   cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE=<path-to-vcpkg>/scripts/buildsystems/vcpkg.cmake
   ```

4. Build the project:
   ```
   cmake --build build
   ```

5. Run the executable from the build directory.

### Alternative Build (Ubuntu/Debian)
If you prefer not to use Vcpkg:
```
sudo apt update
sudo apt install build-essential cmake libglew-dev libglfw3-dev libglm-dev libgl1-mesa-dev
```
Then follow the CMake steps above.

## Research and Physics

This project is based on general relativistic ray tracing techniques. The research paper in `Research/Paper 1.md` provides a comprehensive analysis and proposes enhancements for more accurate Kerr black hole simulation, including:
- Hamilton-Jacobi formalism for geodesic integration
- Carter constant for bound orbits
- Novikov-Thorne accretion disk model
- Relativistic radiative transfer

## References

- Inspired by: [kavan010/black_hole](https://github.com/kavan010/black_hole)
- Research paper: `Research/Paper 1.md`
- General Relativity resources and astrophysics literature

## License

This project is for educational and research purposes. See individual files for licensing information.

## Contributing

This project is currently on hold. Contributions are not being accepted at this time.