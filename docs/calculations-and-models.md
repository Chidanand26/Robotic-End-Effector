# Calculations and models

All values below are calculated, not measured. Measured results belong to Step 13 testing.

## Actuation

Calculated stall force: 154 N per jaw at stall, closed position. The force loop must cap drive at 5 to 10 percent: 8 N is 5.2 percent, 5 N is 3.2 percent. Calculated sweep time: 0.55 s, within the 6 s cycle target. Linkage: crank radius 24 mm, link length 45 mm, jaw travel 90 mm, sweep 20 to 160 degrees.

## Sensing

FSR-408 range 0.2 to 20 N, two sensors, one per finger. Flex sensors 2.2 inch, two, one per finger, for deformation sensing. MLX90614 infrared temperature sensor for object and contact region temperature, with closing prevented at 100 degrees C or above. Four ADC channels are needed, which screened out the 3 ADC option in selection.

## Power

Power budget about 2.1 A at the 12 V input. Supply from 12 V DC through dual buck regulators, 7.4 V and 5 V rails in the calculation model. Note the flag in docs/selection-and-bom.md: the purchased TPS5430D buck is rated 3 A, not the 5 A assumed for the servo rail.

## Models, simulation first

A ROS2 and Gazebo digital twin validates every grasp strategy in simulation before it touches hardware. The Simscape plant is kinematic with no contact model, so the 3 N force loop in the demo lives in the twin, not in the CAD plant.

Local model files, to be uploaded separately as binaries or scripts:

- `VoyagerX_Gripper.slx` and `VoyagerX_Demo.slx` (Simulink)
- `build_voyagerx_requirements.m`: creates VoyagerX_Requirements.slreqx, 42 requirements traced to Review 1 numbers. Remaining manual step: Show Links and link each requirement to its subsystem.
- `build_gripper_arch_v2.m` and twin method note in the MATLAB folder.
- STEP files: `gripper_mechanism.stp`, `for_mathlab.stp`, and the v3 STEP and STL set in `gripper-piper-style/`.

Foundation courses for this work, Handbook Chapter 5.3: Foundations of Robotic Systems, Mechanical Systems Design, 3D Modeling and Analysis, Control Systems, Microcontroller Programming, Analog and Digital Circuits. Concurrent Semester V strengtheners: Robot Analysis and Design, Mechatronics System Design, ROS Lab.
