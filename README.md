# WireViz Designer

A simple web-based tool to visually design cable assemblies and generate WireViz YAML configurations.

## Overview

WireViz Designer is a visual interface that simplifies the creation of WireViz configurations. While WireViz is a powerful tool for documenting cables and wire harnesses, writing YAML configurations manually can be tedious and error-prone. This tool provides a drag-and-drop interface to:

- Create and position connectors
- Define cables with their properties and wire colors
- Visually connect pins to specific cable wires
- Generate a valid WireViz YAML configuration

## Features

### Connectors
- Add connectors with custom names and types
- Define multiple pins for each connector
- Drag and drop connectors to position them
- Edit or delete existing connectors

### Cables
- Create cables with specific properties (name, type, gauge, length)
- Define wire colors using a visual color picker
- Support for both single colors (RD, BK, BU...) and composite colors (WHBU, BUWH...)
- Drag and drop cables to position them
- Edit or delete existing cables

### Connections
- Visual pin-to-wire connections
- Color-coded wires for easy identification
- Click-to-connect interface
- Delete individual connections
- Automatic grouping of related connections in the YAML output

### Combined Colors
- The tool supports combined colors, allowing users to select two colors for a single wire.
- When a combined color is selected, the wire is visually represented with dashed lines showing both colors.
- This feature is useful for representing wires that have dual color coding, enhancing clarity in complex designs.

## Usage

1. **Add Components**
   - Click "Add Connector" to create connectors
   - Click "Add Cable" to create cables
   - Drag components to position them in the design area

2. **Create Connections**
   - Click a pin on a connector
   - Click a wire in a cable
   - Click a pin on another connector to complete the connection

3. **Generate Configuration**
   - Click "Generate YAML" to export the configuration
   - A pop up will open to allow you to copy the YAML to your clipboard or download it as a file
   - The generated file will be downloaded as `wireviz-config.yml`

## Limitations

This tool provides a basic interface for the most common WireViz use cases. It does not support some of WireViz's advanced features such as:

- Shield connections
- Custom wire gauges per connection
- Advanced connector properties
- Notes and additional documentation

The generated YAML can be used as a starting point and manually enhanced with these advanced features if needed.

## Implementation

The tool is implemented as a single HTML file with embedded JavaScript and CSS. It runs entirely in the browser and requires no server-side components or installation.

## Contributing

Feel free to fork this project and enhance it with additional features. Some potential improvements could include:

- Support for more WireViz features
- Better visual representation of connections
- Import existing YAML configurations
- Save/load designs
- Additional validation and error checking

## Related Links

- [WireViz Project](https://github.com/formatc1702/WireViz)

## License

This project is released under the MIT License. 