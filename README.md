# Development of an Application for Radar Measurement Visualization

**Objective:**
To develop an application that reads data from the emulated measurement component of a radar, provided as a Docker image, and displays the detected targets on a plot in polar coordinates.

# Theoretical Information

- **RADAR (Radio Detection and Ranging)**

RADAR is a device used to detect objects and determine their location (distance, azimuth, altitude) and movement using radio waves. The principle of radar operation is based on emitting radio waves and analyzing the signals reflected from objects.

*Main stages of radar operation:*

1) Emission of radio waves: The radar emits radio waves through an antenna. These waves propagate through space until they encounter an object.
2) Reflection of radio waves: When radio waves strike an object (such as an aircraft, ship, or vehicle), they are reflected back towards the radar. The amount and nature of the reflected waves depend on the size, shape, and material of the object.
3) Reception of reflected waves: The reflected radio waves return to the radar and are received by the antenna. The signals are amplified and processed by radar equipment.
Data processing and analysis: The radar analyzes the reflected signals to determine the presence of objects, their distance, direction (azimuth), altitude, and speed. This is achieved by measuring the time it takes for the radio waves to travel from the radar to the object and back, and by analyzing the frequency shift of the signal (Doppler effect) to determine the object's speed.
4) Data visualization: Information about detected objects is displayed on the radar screen, where the operator can track their positions and movements.

- **Key Parameters Determined by Radar**
1) Distance to the object: Measured by the time delay between the moment the signal is emitted and the moment the reflected signal is received.
2) Direction to the object (azimuth and altitude): Determined by the position of the antenna at the moment the reflected signals are received.
3) Object speed: Calculated based on the change in the frequency of the reflected signals (Doppler effect).

# Tasks

**Develop an Application to Display Targets:**

- Develop a web application that connects to the WebSocket server and reads data about detected targets.
- Display the obtained data on a plot in polar coordinates. Consider using the Plotly library or another graphing library.

**Data Processing and Visualization:**

- Process the data received through the WebSocket and display the targets on the plot.
- Each target should be represented as a point on the plot with coordinates (angle, distance).
- Add the ability to change the radar measurement component's parameters using API requests.

**Configuring the Plot:**

- Display distance in kilometers on the radial axis.
- Use different colors or styles for points to indicate different signal power levels returned from the targets.

# Solution

**User interface of the application:**

![image](https://github.com/user-attachments/assets/a8298285-01af-4002-bc68-cfea9d1c1db3)



