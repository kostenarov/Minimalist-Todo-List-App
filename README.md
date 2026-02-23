VOT (Vanilla Online Todo)
VOT is a sleek, high-performance, and minimalist Todo application built using modern web standards. It prioritizes speed and simplicity, offering a distraction-free environment for managing daily tasks.

🚀 Features
Minimalist Design: A clean, responsive interface that works beautifully on mobile and desktop.
Dual-List Organization: Seamlessly transition between "To-do" and "Completed" tasks.
Persistent Storage: Uses browser localStorage to ensure your tasks stay saved even after closing the tab or restarting your computer.
Fluid User Experience:
  Add tasks instantly with the "Enter" key.
  Interactive SVG icons for task manipulation.
  Dynamic empty state messages.
Lightweight Architecture: Zero dependencies or heavy frameworks; built with pure Vanilla JS.
Containerized: Includes a Docker configuration for rapid, consistent deployment via Nginx.

🛠️ Technology Stack
HTML5: Semantic markup for accessible structure.
CSS3: Custom styles featuring the Roboto font family and a mobile-first responsive layout.
Vanilla JavaScript (ES6): Pure logic for DOM manipulation and state management.
Docker: Nginx-based Alpine image for an ultra-small deployment footprint.

📂 Project Structure
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

📦 Getting Started
Local Development
To run this project locally without any specialized tools:
Clone or download this repository.
Open index.html in your favorite web browser.
Running with Docker
If you prefer using Docker for deployment or testing:
Build the image:
'''docker build -t vot-app .

Run the container:
'''docker run -d -p 8080:80 vot-app


Access the app:
Navigate to 'http://localhost:8080' in your browser.

📝 Usage
Add Task: Type your activity in the top input field and press Enter or click the + button.
Complete Task: Click the circular check icon to move a task to the "Completed" section.
Re-activate Task: Click the check icon on a completed item to move it back to the active list.
Delete Task: Click the trash icon to permanently remove an item.

📜 License

This project is open-source and free to use for personal or commercial purposes.
