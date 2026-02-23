# VOT (Vanilla Online Todo)

VOT is a sleek, high-performance, minimalist Todo application built with modern web standards. It prioritizes speed and simplicity, offering a distraction-free environment for managing daily tasks.

## Features

- **Minimalist Design**: Clean, responsive interface that works well on both mobile and desktop
- **Dual-List Organization**: Seamlessly transition between **To-do** and **Completed** tasks
- **Persistent Storage**: Uses browser **localStorage** so tasks stay saved after closing the tab or restarting your computer
- **Fluid User Experience**
  - Add tasks instantly with the **Enter** key
  - Interactive **SVG icons** for task manipulation
  - Dynamic empty-state messages
- **Lightweight Architecture**: Zero dependencies—built with **pure Vanilla JS**
- **Containerized**: Docker configuration for fast, consistent deployment via **Nginx**

## Technology Stack

- **HTML5**: Semantic markup for accessible structure
- **CSS3**: Custom styling (Roboto font family) with a mobile-first responsive layout
- **Vanilla JavaScript (ES6)**: DOM manipulation and state management
- **Docker + Nginx (Alpine)**: Ultra-small deployment footprint

## Project Structure

```text
.
├── index.html              # Main application entry point
├── Dockerfile              # Docker image configuration
├── .editorconfig           # Coding standard configurations
└── resources/
    ├── css/
    │   ├── reset.min.css   # CSS reset for cross-browser consistency
    │   └── style.css       # Main application styles
    └── js/
        └── main.js         # Core application logic & data handling
```

## Getting Started

### Local Development

Run locally without any specialized tools:

1. Clone or download this repository
2. Open `index.html` in your favorite web browser

### Running with Docker

Build the image:

```bash
docker build -t vot-app .
```

Run the container:

```bash
docker run -d -p 8080:80 vot-app
```

Open the app:

- Visit: http://localhost:8080

## Usage

- **Add Task**: Type your task in the top input field and press **Enter** (or click the **+** button)
- **Complete Task**: Click the circular **check** icon to move a task to **Completed**
- **Re-activate Task**: Click the **check** icon on a completed item to move it back to **To-do**
- **Delete Task**: Click the **trash** icon to permanently remove an item

## License

This project is open-source and free to use for personal or commercial purposes.