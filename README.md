# WebApp for ABB OmniCore FlexPendant

This repository contains a WebApp designed for the ABB OmniCore FlexPendant, implemented in JavaScript and HTML. The WebApp enables control of controller inputs and outputs for the ABB system, allowing users to interact with machine signals and monitor processes directly from the FlexPendant interface. In this case the application is a coffe serving control, with nine different button funcionalities.


![App_Icon](./AppIcon.png)

## Overview

The WebApp provides the following key functionalities:
- **Speed Reduction and Stop Signals**: Allows control over speed signals in Safety Speed Monitoring (SSM) mode.
- **Process Start Signal**: Activates the main procedure through an interactive button.
- **Process Visualization**: Displays the count of completed tasks, such as prepared items, directly on the interface.

## Implementation Details

- **JavaScript**: Defines the core behavior of the application, including dynamic creation of interactive elements (buttons) that control various signals. These buttons are implemented with attribute classes provided by the ABB Omnicore SDK.
  
- **HTML**: Structures the WebApp interface, using a cell-based layout where elements are organized within predefined classes from the Omnicore SDK. Each cell includes labels and interactive components linked to JavaScript functions for a seamless experience on the FlexPendant.

## Installation

1. Place all WebApp files in the `HOME` directory of the ABB OmniCore controller. This ensures compatibility and proper access from the FlexPendant.
2. Open the application on the FlexPendant to control signals and monitor station statuses in real-time.

> Replace `./path_to_gif.gif` with the actual path of the GIF showing the WebApp in action.

## File Structure

- `index.html`: Defines the HTML structure for the WebApp interface.
- `app.js`: Contains the JavaScript code for handling button actions and signal control.
- `styles.css`: Optional CSS file for custom styling.

## Dependencies

The WebApp relies on ABB's Omnicore SDK for JavaScript and HTML element classes, which facilitate seamless integration with the FlexPendant environment.

## Additional Information

The full JavaScript and HTML code for this WebApp can be found in the `annexes` folder of this repository, providing all details for customization and further development.


Attention: It is neccessary to check if the "Access Level" of the signals aimed to control is established to "All" instead of "Default"
The "Access Level" parameter can be set up from RobotStudio Controller->Configuration->I/O System->Signal
