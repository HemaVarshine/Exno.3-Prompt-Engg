# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:15/5/2025                                                                           
### REGISTER NUMBER : 212222060082
### Aim:
To prompt an AI assistant to generate different types of outputs that assist in the design, control, and deployment of a remote-controlled robot used for surveillance in hazardous environments (e.g., disaster zones, military, or industrial inspections).

### Procedure: 
To design a remote-controlled robot, a structured approach using scenario-based prompting techniques is crucial. This procedure ensures the robot design addresses both technical functionality and user interaction requirements in different environments. The following steps use varied prompting strategies to guide the development process at each stage.

### Project Overview
To design a remote-controlled robot, start by defining its core functions, such as navigating rough terrain and detecting obstacles, using zero-shot prompting. Next, choose appropriate sensors like LiDAR, cameras, and ultrasonic sensors for obstacle detection, using one-shot prompting. Develop control algorithms with real-time feedback, incorporating few-shot prompting for decision-making. Use chain-of-thought prompting to refine pathfinding algorithms that ensure smooth movement in dynamic environments. Implement a wireless communication system to allow remote control, guided by instruction-based prompting. Finally, test and optimize the system based on user feedback for improved functionality and user experience.

### Prompting Techniques for Each Stage of the Design Process Stage 

### 1.Zero-shot prompting
OBJECTIVE :Ask the model to perform a task without any examples.
PROMPT :"Describe how a remote-controlled robot can navigate rough terrain."
RESPONSE :A remote-controlled robot navigates rough terrain using all-terrain wheels or tracks, a suspension system, and sensors like IMUs and cameras.

### 2.One-shot prompting
OBJECTIVE :Provide one example before asking the model to perform a similar task.
PROMPT :"Here is an example of a robot arm picking up an object. Now explain how a robot camera can track a moving object."
RESPONSE :A robot camera tracks a moving object by continuously capturing video frames, using computer vision algorithms (like object detection and optical flow) to locate the object in real time, and adjusting the camera's position to keep it in focus.


### 3.Few-shot prompting
OBJECTIVE :Provide a few examples before asking for a similar response.
PROMPT :"Example 1: Robot detects fire and sends alert. Example 2: Robot detects gas leak and activates ventilation. Now give another example of hazard detection."
RESPONSE :Example 3: Robot detects high radiation levels and shuts down nearby equipment.

### 4.Instruction prompting
OBJECTIVE :Directly tell the model what to do clearly.
PROMPT :"Write a Python script to control a robot using Bluetooth commands."
RESPONSE :import bluetooth
          robot_address = 'XX:XX:XX:XX:XX:XX'  # Replace with actual address 
          sock = bluetooth.BluetoothSocket(bluetooth.RFCOMM)
          sock.connect((robot_address, 1))
          def send_command(command):
          sock.send(command)

### 5.Role prompting
OBJECTIVE :Ask the model to play a specific role or perspective.
PROMPT :"Act as a robotics engineer. Design a module to control a robot's movement through a smartphone."
RESPONSE :To improve obstacle detection, sensor fusion can be used by combining data from LiDAR, ultrasonic sensors, and cameras for greater accuracy. The pathfinding can be enhanced using a dynamic A* algorithm that updates based on real-time sensor input. 

### 6.Refinement prompting
OBJECTIVE :Ask the model to improve or refine a previous output.
PROMPT :"Improve this robot pathfinding algorithm for better obstacle detection."
RESPONSE :To improve this robot pathfinding algorithm for better obstacle detection, implement sensor fusion by combining inputs from LiDAR, ultrasonic sensors, and cameras to enhance accuracy


# Result: Thus the Prompts were exected succcessfully .

