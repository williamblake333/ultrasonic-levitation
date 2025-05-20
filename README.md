# Ultrasonic Levitator Project

![Acoustic Levitator in Action](videos/medialevitator-demo-video.mov)

## Overview

This repository contains the designs, source code, and documentation for building your own ultrasonic/acoustic levitator. This device uses ultrasonic waves to create standing wave patterns that can suspend small objects in mid-air.

## Features

- Suspends small objects (up to 3-5mm) in mid-air using sound waves
- Uses readily available 40kHz ultrasonic transmitters
- Based on Arduino R4 Minima for precise timing control
- Modular design allows for expansion to multi-axis configurations
- Fully open-source hardware and software

## Demo

[Watch the levitator in action (Video)](link_to_your_video)

## Getting Started

- [Materials List](documentation/materials_list.md)
- [Assembly Guide](documentation/assembly_guide.md)
- [Programming Guide](documentation/programming_guide.md)

## How It Works

The acoustic levitator creates standing waves between two arrays of ultrasonic transmitters. Objects can be suspended at the nodes of these standing waves, where the acoustic radiation pressure balances the force of gravity.

For a detailed explanation of the physics behind acoustic levitation, see [The Science of Acoustic Levitation](documentation/science_explanation.md).

## Hardware

The design files for 3D printable parts are available in the [3D Models](hardware/3d_models) directory.

## Software

The Arduino code for controlling the acoustic levitator is available in the [Source Code](src) directory.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.

## Acknowledgments

- [Name any people or resources that inspired or helped with the project]
