
# ROS2 Joystick for Turtlesim with NiceGUI Integration

This project provides a simple joystick that controls the `turtlesim_node` in ROS2, enhanced with a GUI powered by NiceGUI. It complements the ROS2 Turtlesim tutorial and demonstrates how to interact with the Turtlesim environment using both a joystick and a graphical interface.

## Features

- **Joystick Control**: Control the Turtlesim turtle using a joystick, with commands sent only when the joystick input changes.
- **GUI Interface**: Integrated with NiceGUI for an easy-to-use graphical interface.
- **Event-driven Commands**: Efficient command handling by sending new twist commands only on joystick input changes.
- **ROS2 Compatibility**: Fully compatible with ROS2, specifically tested with the Humble distribution.

## Prerequisites

Before running this project, ensure you have the following installed:

- **ROS2 Humble**: The project is built and tested on ROS2 Humble.
- **Turtlesim Package**: Turtlesim is a lightweight simulator included with ROS2.
- **NiceGUI**: A simple, powerful GUI framework for Python.

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/ros2_joystick.git
   cd ros2_joystick
   ```

2. **Build the package**:

   Navigate to your ROS2 workspace and build the package:

   ```bash
   colcon build --packages-select ros2_joystick
   ```

3. **Source your workspace**:

   ```bash
   source install/setup.bash
   ```

4. **Install NiceGUI**:

   Install NiceGUI using pip for GUI integration:

   ```bash
   pip install nicegui
   ```

## Usage

To use the joystick control with Turtlesim and the NiceGUI interface, follow these steps:

1. **Start the joystick node**:

   In the first terminal, run the joystick node:

   ```bash
   ros2 run ros2_joystick joystick
   ```

2. **Start the Turtlesim node**:

   In the second terminal, start the Turtlesim node:

   ```bash
   ros2 run turtlesim turtlesim_node
   ```

3. **Control the turtle**:

   Use your joystick to control the turtle in the Turtlesim window. The turtle will move based on the joystick input, and the node will send new twist commands only when there is a change in the joystick position.

4. **Launch the GUI (if applicable)**:

   If your project includes GUI components using NiceGUI, run the GUI as instructed in your code. This step may vary depending on your specific implementation.

## Customization

- **Joystick Configuration**: Modify the joystick settings in the `joystick` node to match your hardware.
- **GUI Customization**: Customize the NiceGUI interface to suit your needs.
- **Command Frequency**: Adjust the node to send commands at a different rate by modifying the code.

## License

This project is licensed under the Apache 2.0 License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Feel free to fork the repository, make changes, and submit a pull request. Whether it’s code, documentation, or suggestions, your input is valuable.

## Acknowledgments

- **ROS2 Team**: For creating a robust platform for robotics development.
- **Turtlesim**: For being an excellent tool for learning and testing ROS2 concepts.
- **NiceGUI**: For providing a simple and powerful GUI framework for Python.

---
