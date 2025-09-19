# API Reference

## Methods

### ServoLib_GenerateServo(servo_model, xcenter, zcenter)

This method generates a basic model of the specified servo.
The generated model is intended to be a guide for designing around servo hardware. It is not intended to be accurate beyond the basic measurements.

The method accepts the following parameters:

- `servo_model` - the name of the servo to model.
- `xcenter` - specifies where the motor should be centered horizontally (defaults to "axle")

  - "axle" generates the motor centered on the axle.
  - "body" generates the motor with the body centered along the origin.

- `zcenter` - determines where the motor is positioned on the z-axis (defaults to "axle top").
  - "axle top" or "top" generates the motor with the top of the axle on the XY plane.
  - "axle base" or "body top" or "motor top" generates the motor with the bottom of the axle on the XY plane.
  - "wing top" generates the motor with the top of the wings on the XY plane.
  - "wing bottom" generates the motor with the bottom of the wings on the XY plane.
  - "body base" or "base" or "motor bottom" generates the motor with the entire servo above the XY plane.

### ServoLib_GenerateBodyOutline(servo_model, xcenter)

This method generates an outline of the body of the selected servo.

The method accepts the following parameters:

- `servo_model` - the name of the servo to model

- `xcenter` - specifies where the motor should be centered horizontally (defaults to "axle")
  - "axle" generates the motor centered on the axle.
  - "body" generates the motor with the body centered along the origin.

### ServoLib_GenerateScrewHolesOutline(servo_model, xcenter)

Generates a 2D hole pattern for the servo's mounting screw holes.
This pattern can be extruded to create mounting screw holes in your model.

The method accepts the following parameters:

- `servo_model` - the name of the servo to model.
- `xcenter` - specifies where the motor should be centered horizontally (defaults to "axle")
  - "axle" generates the motor centered on the axle.
  - "body" generates the motor with the body centered along the origin.

### ServoLib_GenerateWingOutline(servo_model, xcenter)

This method generates an outline of the wings of the selected servo.

The method accepts the following parameters:

- `servo_model` - the name of the servo to model
- `xcenter` - specifies where the motor should be centered horizontally (defaults to "axle")
  - "axle" generates the motor centered on the axle.
  - "body" generates the motor with the body centered along the origin.

## Functions

### ServoLib_ServoModelIsValid(servo_model)

Returns true if servo_model is a recognized Servo Model Name.
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_AftHeight(servo_model)

Returns the Aft Height of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_WingHeight(servo_model)

Returns the Wing Height of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_ForeHeight(servo_model)

Returns the Fore Height of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_AxleHeight(servo_model)

Returns the Axle Height of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_BodyWidth(servo_model)

Returns the Body Width of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_WingWidth(servo_model)

Returns the Wing Width of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_AxleOffset(servo_model)

Returns the Axle Offset of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_AxleDiameter(servo_model)

Returns the Axle Diameter of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_BodyLength(servo_model)

Returns the Body Length of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_BodyHeight(servo_model)

Returns the Body Height of the specified servo model (see [measurements documentation](measurements.md)).
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.

### ServoLib_SplineType(servo_model)

Returns the Spline Type of the specified servo model.
The function accepts the following parameters:

- `servo_model` - the name of the servo to model.
