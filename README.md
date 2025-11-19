# D3.js Fishbone Diagram Creator

An interactive web application for creating fishbone diagrams (Ishikawa diagrams) with drag-and-drop timeline reordering capabilities.

## Features

- **Interactive Fishbone Diagrams**: Create cause-and-effect analysis diagrams with a clean, modern interface
- **Flexible Timeline**: Fins are automatically arranged chronologically based on creation order
- **Drag-and-Drop Reordering**: Easily reorder causes by dragging fins in the control panel
- **Top and Bottom Fins**: Add causes to both sides of the fishbone spine
- **Descriptions**: Include optional detailed descriptions for each cause
- **Real-time Updates**: Diagram updates instantly as you add, remove, or reorder fins
- **Responsive Design**: Adapts to different screen sizes

## What is a Fishbone Diagram?

A fishbone diagram (also known as an Ishikawa diagram or cause-and-effect diagram) is a visualization tool used to systematically identify and organize potential causes of a problem or effect. The diagram resembles a fish skeleton, with the problem statement at the "head" and various causes branching off like "bones."

## Usage

### Getting Started

1. Open `index.html` in a modern web browser
2. No build process or dependencies to install - it works out of the box!

### Creating a Diagram

1. **Set the Main Effect**: Enter your problem or effect statement in the "Main Effect" section
2. **Add Fins**: Use the "Add Top Fin" or "Add Bottom Fin" sections to add causes
   - Enter a label (e.g., "Materials", "Methods", "People")
   - Optionally add a description for more detail
3. **Reorder Fins**: Drag and drop fins in the lists to change their timeline sequence
4. **Remove Fins**: Click the "Delete" button on any fin to remove it

### Timeline Behavior

The diagram combines fins from both top and bottom lists into a single chronological timeline based on when they were created. This allows you to:
- Mix related causes from different categories
- Maintain temporal relationships between causes
- Visualize the sequence of contributing factors

## Technical Details

### Technologies Used

- **D3.js v7**: For SVG rendering and data visualization
- **Vanilla JavaScript**: No framework dependencies
- **CSS3**: Modern styling with gradients and transitions
- **HTML5 Drag and Drop API**: For interactive reordering

### Browser Support

Works in all modern browsers that support:
- ES6 JavaScript
- SVG
- CSS Grid and Flexbox
- HTML5 Drag and Drop API

### File Structure

```
simpleFishbone/
├── index.html          # Complete application (HTML + CSS + JavaScript)
└── README.md          # This file
```

## Customization

The application is contained in a single HTML file, making it easy to customize:

- **Colors**: Modify the CSS gradient values and color variables
- **Layout**: Adjust margin, padding, and size values in the styles
- **Diagram Spacing**: Change `finLength`, `finAngle`, and spacing calculations in the `drawFishbone()` function
- **Text Styling**: Modify font sizes and weights in the CSS classes

## Common Use Cases

- Root cause analysis
- Quality control and problem-solving
- Process improvement
- Risk analysis
- Brainstorming sessions
- Six Sigma projects
- Manufacturing defect analysis

## License

Feel free to use and modify this tool for your projects.

## Contributing

This is a simple single-file application. To contribute:
1. Fork the repository
2. Make your changes to `index.html`
3. Test in multiple browsers
4. Submit a pull request

## Development

No build process required. Simply edit `index.html` and refresh your browser to see changes.

### Key Functions

- `addFin(position)`: Adds a new fin to top or bottom
- `removeFin(position, id)`: Removes a fin by ID
- `drawFishbone()`: Renders the SVG diagram using D3.js
- `handleDragStart/Drop/End()`: Manages drag-and-drop reordering

## Credits

Built with D3.js - a JavaScript library for producing dynamic, interactive data visualizations.
