# Acoustic Levitator Assembly Guide

This guide provides step-by-step instructions for assembling your acoustic levitator.

## 1. 3D Printing the Components

1. Download the STL files from the [3D Models](../hardware/3d_models) directory
2. Print the components according to the recommended settings
3. Clean up any support material and check that all mounting holes are clear

## 2. Preparing the Ultrasonic Transmitters

1. Sort your transmitters, ensuring you're using only the "T" (transmitter) units
2. For each transmitter, solder a red wire to the positive terminal and a black wire to the negative terminal
3. Use heat shrink tubing to insulate the connections
4. Test each transmitter with a multimeter to ensure proper connections

## 3. Mounting Transmitters to Platforms

1. Insert each transmitter into its designated hole in the platform
2. Ensure all transmitters are facing the same direction (emitting side toward the center)
3. Secure transmitters with a small amount of hot glue if needed

## 4. Wiring the Transmitters in Parallel

### Top Platform
1. Connect all positive (red) wires from the top platform transmitters together
2. Connect all negative (black) wires from the top platform transmitters together
3. Add longer lead wires to these two connection points for connecting to the L298N

### Bottom Platform
1. Connect all positive (red) wires from the bottom platform transmitters together
2. Connect all negative (black) wires from the bottom platform transmitters together
3. Add longer lead wires to these two connection points for connecting to the L298N

## 5. Connecting to the L298N Motor Driver

1. Connect the top platform's positive lead to L298N OUT1
2. Connect the top platform's negative lead to L298N OUT2
3. Connect the bottom platform's positive lead to L298N OUT3
4. Connect the bottom platform's negative lead to L298N OUT4

## 6. Connecting L298N to Arduino R4 Minima

1. Connect Arduino pin A0 to L298N IN1
2. Connect Arduino pin A1 to L298N IN2
3. Connect Arduino pin A2 to L298N IN3
4. Connect Arduino pin A3 to L298N IN4
5. Connect Arduino 5V to both ENA and ENB pins on the L298N
6. Connect Arduino GND to L298N GND
7. Connect power supply positive to L298N VCC
8. Connect power supply negative to L298N GND

## 7. Assembling the Support Structure

1. Attach the support structure to the bottom platform using M3 screws
2. Mount the fine adjustment mechanism to the support structure
3. Attach the top platform to the fine adjustment mechanism
4. Ensure both platforms are parallel to each other

## 8. Programming the Arduino

1. Connect the Arduino R4 Minima to your computer
2. Open the Arduino IDE
3. Load the `single_axis_levitator.ino` sketch from the repository
4. Upload the sketch to the Arduino

## 9. Tuning and Testing

1. Set the initial spacing between platforms to approximately 25mm
2. Power on the system
3. Use an oscilloscope to verify the 40kHz signal if available
4. Adjust the platform spacing using the fine adjustment mechanism
5. Test with a small piece of expanded polystyrene (1-3mm)
6. Fine-tune the spacing until stable levitation is achieved

## Troubleshooting

If you encounter issues, refer to the [Troubleshooting Guide](troubleshooting.md).

## Next Steps

Once your basic levitator is working, consider:
1. Experimenting with different objects for levitation
2. Measuring the exact node positions
3. Upgrading to a three-axis system for more stable levitation
