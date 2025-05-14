# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:5/5/25                                                                           
### REGISTER NUMBER : 212222060082
### Aim:
To prompt an AI assistant to generate different types of outputs that assist in the design, control, and deployment of a remote-controlled robot used for surveillance in hazardous environments (e.g., disaster zones, military, or industrial inspections).

### AI Tools Used: 
• AI Development Platforms: OpenAI API for natural language processing (NLP) and GPT
based responses. 
• Data Collection Tools: Google Forms for customer survey data, chatbot logs for 
conversational analysis

### Procedure:
To design a remote-controlled robot, start by defining its core functions, such as navigating rough terrain and detecting obstacles, using zero-shot prompting. Next, choose appropriate sensors like LiDAR, cameras, and ultrasonic sensors for obstacle detection, using one-shot prompting. Develop control algorithms with real-time feedback, incorporating few-shot prompting for decision-making. Use chain-of-thought prompting to refine pathfinding algorithms that ensure smooth movement in dynamic environments. Implement a wireless communication system to allow remote control, guided by instruction-based prompting. Finally, test and optimize the system based on user feedback for improved functionality and user experience.

### Algorithm:  
1.PROMPT PATTERN : Zero Shot prompting
  PROMPT         :"Describe how a remote-controlled robot can navigate rough terrain."
  RESPONSE       :A remote-controlled robot navigates rough terrain using all-terrain wheels or tracks, a suspension system, and sensors like IMUs and cameras. These help 
  maintain balance, detect obstacles, and allow the operator to control it effectively in uneven environments.

2. PROMPT PATTERN :One shot Prompting
   PROMPT         :"Here is an example of a robot arm picking up an object. Now explain how a robot camera can track a moving object."
   RESPONSE       : A robot camera tracks a moving object by continuously capturing video frames, using computer vision algorithms (like object detection and optical flow) 
   to locate the object in real time, and adjusting the camera's position to keep it in focus.

3. PROMPT PATTERN : Few Shot Prompting
   PROMPT         :"Example 1: Robot detects fire and sends alert,Example 2: Robot detects gas leak and activates ventilation,Now give another example of hazard detection."
   RESPONSE       :Example 3: Robot detects high radiation levels and shuts down nearby equipment.

4. PROMPT PATTERN :Chain-of-thought Prompting
   PROMPT         :"Explain step by step how a robot can identify a human in its path and avoid collision."
   RESPONSE       :  Step 1: The robot uses sensors like LiDAR, cameras, or infrared to scan its surroundings.
                     Step 2: The robot processes the sensor data using object detection algorithms to identify a human.                  
                     Step 3: Once a human is detected, the robot calculates the distance and trajectory.
                     Step 4: The robot compares its path with the human's position and plans an alternative route.
                     Step 5: The robot then adjusts its speed or changes direction to avoid a collision.

5. PROMPT PATTERN :Instruction Prompting
   PROMPT         :"Write a Python script to control a robot using Bluetooth commands."
   RESPONSE       : import bluetooth
                    robot_address = 'XX:XX:XX:XX:XX:XX'  # Replace with actual address
                    # Connect to robot
                     sock = bluetooth.BluetoothSocket(bluetooth.RFCOMM)
                    sock.connect((robot_address, 1))
                    # Send commands to robot
                    def send_command(command):
                    sock.send(command)
                    # Example commands to control robot
                    send_command('FORWARD')
                    send_command('BACKWARD')
                    # Close connection
                    sock.close()

6. PROMPT PATTERN : Refinement Based Prompting
   PROMPT         :"Improve this robot pathfinding algorithm for better obstacle detection."
   RESPONSE       :  To improve obstacle detection, we can add sensor fusion and enhance the pathfinding algorithm as follows:
                     Sensor Fusion: Combine data from LiDAR, ultrasonic sensors, and cameras for more accurate obstacle detection.
                     Enhanced Algorithm: Implement the A* algorithm with dynamic obstacle avoidance, considering real-time sensor data to update the robot's path.
                     Real-time Feedback: Continuously adjust the robot's path based on immediate environmental changes (e.g., objects moving or new obstacles appearing).


# Result: Thus the Prompts were exected succcessfully .

