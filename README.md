
Historical Archive Search System 
Project Overview
The Historical Archive Search System is a Retrieval-Augmented Generation (RAG)-based intelligent document retrieval platform designed to modernize access to historical archives. This interactive demo showcases the key features and capabilities of the system using a fully functional web interface.

Key Features Demonstrated
Semantic Search Engine

Advanced search capabilities for historical documents

Sample queries and search suggestions

Real-time search results with animations

Three View Modes

Grid View: Card-based document display with metadata

Timeline View: Chronological arrangement of documents

Knowledge Graph View: Interactive visualization of entity relationships

AI-Powered Features

ScaleDown compression simulation

Context restoration demonstration

Handwriting OCR capabilities

Entity extraction and linking

Interactive Filters

Time period filtering (1600-1950)

Document type selection

Entity-based filtering

AI feature toggles

File Structure
text
single-file-demo.html
├── HTML Structure
│   ├── Header with animated title
│   ├── Sidebar with interactive filters
│   ├── Main content area with search
│   └── Footer with links
├── CSS Styles
│   ├── Custom color palette for historical theme
│   ├── Responsive design for all screen sizes
│   ├── Animations and transitions
│   └── Custom fonts (Cinzel, Lora, Open Sans)
└── JavaScript Functions
    ├── Document data management
    ├── View switching logic
    ├── Filter application system
    └── Interactive animations
Technologies Used
HTML5: Semantic structure and content

CSS3: Styling, animations, and responsive design

Vanilla JavaScript: Interactive functionality

Font Awesome: Icons for UI elements

Google Fonts: Typography (Cinzel, Lora, Open Sans)

How to Use the Demo
Searching Documents

Enter a query in the search box (e.g., "Irish famine letters")

Click "Semantic Search" or press Enter

Use "Sample Query" for suggested searches

Applying Filters

Use the sidebar to filter by time period

Select specific document types

Choose entity types to include

Toggle AI features on/off

Click "Apply Filters" to update results

Switching Views

Grid View: Card-based display (default)

Timeline View: Chronological timeline

Graph View: Interactive knowledge graph

Interacting with Elements

Hover over document cards for 3D effects

Click on timeline items for details

Click on graph nodes to explore relationships

Use collapsible filter sections

Animation System
The demo includes several CSS animations:

Page Load Animations

fadeInDown: Header entry

slideInLeft: Sidebar and logo

fadeIn: Main content area

fadeInUp: Search box and results

Interactive Animations

pulse: Highlighting elements

float: Graph node animation

spin: Loading spinner

Hover effects: 3D card tilt, button lifts

Staggered Animations

Document cards appear sequentially

Timeline items fade in with delays

Graph nodes animate with offsets

Sample Data
The demo includes 6 historical documents covering:

Irish Famine (1847)

Industrial Revolution (1832)

American Revolution (1776)

Women's Suffrage (1908)

World War I (1916)

Civil Rights Movement (1963)

Each document includes:

Title and document type

Historical date

Sample content

Extracted entities (people, places, events)

Citation information

Knowledge Graph
The interactive graph visualizes relationships between:

People: Historical figures

Places: Geographical locations

Events: Historical events

Documents: Archival materials

Features:

Dynamic node placement

Animated connections

Interactive node selection

Relationship exploration

Responsive Design
The interface works on:

Desktop: Full sidebar + main content layout

Tablet: Adaptive grid layouts

Mobile: Stacked layout with full-width elements

Breakpoints:

1024px: Switches to column layout

768px: Single-column grid, simplified features

Customization Options
Color Scheme

Primary dark: #2c3e50

Accent gold: #d4af37

Paper backgrounds: #f5eedc, #f8f3e6

Entity colors: Green (people), Red (places), Blue (events)

Typography

Cinzel: Headers and titles

Lora: Document content

Open Sans: UI elements and body text

Animation Timing

Page load: 1-1.5 second sequences

Interactive: 0.3-0.5 second transitions

Delays: Staggered 0.1-0.6 second offsets

Extending the Demo
To add more documents:

javascript
const newDocument = {
    id: 7,
    title: "Your Document Title",
    type: "letter", // or "newspaper", "manuscript"
    typeIcon: "fas fa-envelope", // matching icon class
    date: "YYYY",
    content: "Document content here...",
    entities: [
        {type: "person", name: "Name"},
        {type: "place", name: "Location"},
        {type: "event", name: "Event"}
    ],
    citation: "Source citation"
};
To modify the knowledge graph:

javascript
const newNode = {
    id: 9,
    type: "person", // "person", "place", "event", "document"
    label: "Node Label",
    x: 100, // Position X
    y: 100  // Position Y
};

const newConnection = {
    from: 1, // Starting node ID
    to: 9    // Ending node ID
};
Browser Compatibility
Tested and working on:

Chrome 90+

Firefox 88+

Safari 14+

Edge 90+

Performance Notes
Optimizations

CSS animations use transform and opacity for GPU acceleration

JavaScript uses event delegation for efficient event handling

Images are SVG patterns for minimal file size

Memory Management

No external dependencies to load

All data contained in a single file

Clean event listeners and timeouts

System Requirements
To run the demo:

Modern web browser

Internet connection (for fonts and icons)

5MB+ of free memory

Deployment
Simply open the HTML file in any modern web browser. No server or compilation required.

Known Limitations
Demo Constraints

Contains only 6 sample documents

Search functionality is simulated

No actual OCR or AI processing

Static knowledge graph

Browser Support

CSS Grid required for layout

ES6 JavaScript features used

CSS Custom Properties (variables)

Future Enhancements
Potential additions to extend the demo:

Dynamic Data Loading

JSON file integration for documents

API simulation with fetch()

Local storage for user preferences

Advanced Interactions

Document zoom and pan

Timeline scrubbing

Graph node dragging

Additional Features

User authentication simulation

Document upload preview

Search history

Troubleshooting
Common issues and solutions:

Animations not working

Ensure browser supports CSS animations

Check for JavaScript errors in console

Layout issues

Clear browser cache

Check browser zoom level (should be 100%)

Fonts not loading

Check internet connection

Allow external resources in browser



