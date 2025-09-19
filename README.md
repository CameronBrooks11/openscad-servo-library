# Servo Library for OpenSCAD

An OpenSCAD library for creating designs that incorporate standard servos.

Created by Brad Kartchner (<kartchnb@gmail.com>)

## Quick Start

```c
include <servo_lib.scad>

// Generate a servo model
ServoLib_GenerateServo("SG90 (Clone)");

// Get servo dimensions
body_width = ServoLib_BodyWidth("SG90 (Clone)");
body_height = ServoLib_BodyHeight("SG90 (Clone)");
```

## Supported Servos

Current supported servo models:

- "S3003 (Clone)"
- "MG90S (Clone)"
- "SG90 (Clone)"
- "GH-S37D"

## Documentation

- **[API Reference](docs/api.md)** - Complete method and function documentation
- **[Measurements](docs/measurements.md)** - Servo measurement diagrams and descriptions
- **[Changelog](docs/changelog.md)** - Version history

## License

This library is provided as-is for use in your OpenSCAD projects.
