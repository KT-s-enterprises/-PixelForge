# -PixelForge
A web-based image editor allowing users to upload, apply basic transformations, adjustments, and filters, then download their modified images.

file structure

PixelForge/
├── public/
│   └── index.html
├── src/
│
├── assets/
│   └── icons/, images/         # Icons, placeholders, and local assets
│
├── components/
│   ├── CanvasEditor.jsx        # Core canvas and image rendering
│   ├── SidebarControls.jsx     # UI controls (rotate, flip, sliders)
│   ├── HistoryControls.jsx     # Undo/Redo buttons
│   ├── FilterControls.jsx      # Grayscale, Sepia, Invert buttons
│   ├── AdjustmentSliders.jsx   # Brightness, Contrast, Saturation
│   ├── AIControls.jsx          # AI-specific buttons (Remove BG, Enhance)
│   ├── DownloadButton.jsx      # Download edited image
│   └── ToolPanel.jsx           # Text, Draw, Crop, Layers
│
├── context/
│   ├── EditorContext.js        # Context for global editor state
│   └── HistoryReducer.js       # Reducer for undo/redo stack
│
├── hooks/
│   └── useCanvasUtils.js       # Custom hook for canvas operations
│
├── utils/
│   ├── imageUtils.js           # Brightness, contrast, filters logic
│   ├── transformUtils.js       # Flip, rotate, crop logic
│   ├── aiUtils.js              # AI tasks (remove BG, OCR, etc.)
│   └── download.js             # Image export/download logic
│
├── styles/
│   └── main.css                # Global styles (Tailwind or CSS Modules)
│
├── App.jsx                     # Root component
├── main.jsx                    # Entry point (ReactDOM.render)
├── index.css                   # Tailwind base styles or resets
└── package.json
