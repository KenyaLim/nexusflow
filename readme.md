Nexus Flow Pro - Visual Logic Engine

Nexus Flow Pro is an advanced, vanilla JavaScript implementation of a node-based visual programming interface. It demonstrates complex DOM manipulation, SVG Bezier curve math, infinite canvas transformations, and a simulated asynchronous execution engine.

Live Demo: Simply open index.html in your browser. No build steps required.

🚀 Features

Infinite Canvas: Middle-mouse drag (or Alt+Click drag) to pan, and scroll-wheel to zoom. The grid scales and translates seamlessly using CSS Matrix transformations.

Object-Oriented Architecture: Written in vanilla JS but structured like a modern modular app (CanvasController, GraphManager, ExecutionEngine).

Dynamic SVG Wiring: Mathematical cubic-bezier curves drawn in real-time connecting node ports, adjusting tension based on distance.

Live Execution Engine: A fully functional traversal engine. Nodes can process data, apply math operations, and pass data down the chain with simulated asynchronous delays and glowing visual feedback.

Local Storage Persistence: The graph layout and state are automatically serialized and saved to localStorage. Refreshing the page restores your exact workspace.

Context Menus: Right-click the canvas to spawn nodes, or right-click a node to delete it.

Interactive Properties Panel: Selecting a node dynamically generates input fields to modify that specific node's internal state (e.g., changing math operators or string values).

🛠️ Technical Implementation Highlights

This project intentionally avoids heavy frameworks (React, Vue) or canvas libraries (Fabric.js, LiteGraph) to serve as a pure demonstration of core web technologies.

Single File Architecture: All HTML, Tailwind CSS setup, and JavaScript logic is consolidated into a single highly-structured file for ultimate portability.

Drag & Drop: Bypasses the clunky native HTML5 drag-and-drop API for nodes. Uses precise mousedown/mousemove event listeners with coordinate translation mapping clientX/clientY screen space into transformed canvas world space.

State Management: The GraphManager class maintains a single source of truth for the graph structure, abstracting DOM updates away from data changes.

📦 How to Use

Clone this repository.

Open index.html in any modern web browser.

Add Nodes: Drag nodes from the left library into the canvas, or right-click the canvas.

Connect: Click and hold on an output port (right side of a node), drag the wire, and drop it on an input port.

Configure: Click a node to open the properties panel on the right.

Execute: Click the green "Execute" button in the top right to watch data flow through your logic graph and print to the bottom-right console.

🔧 Node Types Included

Start Trigger: The entry point for the execution flow.

String / Number Value: Static data generators.

Math Operation: Takes an input, applies logic (Add/Multiply) against an internal factor, and outputs the result.

Log to Console: Terminal output node to view the final processed data.

👨‍💻 Author

Created as a portfolio demonstration of advanced frontend engineering and interactive UI development.
